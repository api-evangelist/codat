# Codat GraphQL Schema

## Overview

Codat is a unified API platform providing standardized access to SMB financial data from 30+ accounting, banking, commerce, and ERP systems. This conceptual GraphQL schema represents the Codat data model across its Platform, Lending, Bank Feeds, Sync for Expenses, Sync for Commerce, Sync for Payroll, and Sync for Payables APIs.

Codat's REST API surface covers company management, data connections, pull/push operations, and standardized financial data objects. This schema translates that model into GraphQL types for query and mutation use cases.

## Schema Source

- API Reference: https://docs.codat.io/reference/
- Platform API: https://docs.codat.io/platform-api
- Lending API: https://docs.codat.io/lending-api
- Bank Feeds API: https://docs.codat.io/bank-feeds-api
- OpenAPI Source: https://github.com/codatio/oas
- GitHub Organization: https://github.com/codatio

## Type Categories

### Platform & Core

- **Company** — A business entity registered in Codat; the top-level organizational unit for all financial data.
- **Connection** — A link between a Company and a source accounting, banking, or commerce platform.
- **Dataset** — A collection of data pulled from a Connection for a specific data type.
- **Integration** — A supported third-party platform (e.g., QuickBooks, Xero, Plaid) that Codat connects to.
- **PullOperation** — Represents an asynchronous data pull request for a given data type from a Connection.
- **DataStatus** — The sync status of a particular data type for a given Connection.
- **Webhook** — An event notification registered to receive Codat platform events.
- **Setting** — Configuration options applied at the company, connection, or platform level.

### Accounting — Transactions

- **AccountingAccount** — A chart-of-accounts entry representing a general ledger account.
- **AccountTransaction** — A raw transaction record from a bank account linked in accounting software.
- **Bill** — A supplier invoice recorded in accounting software representing money owed by the company.
- **BillCreditNote** — A credit issued against a Bill, reducing the amount owed to a supplier.
- **BillPayment** — A payment record applied against one or more Bills.
- **CreditNote** — A credit document issued to a customer, reducing the amount they owe.
- **DirectCost** — A cost not associated with a bill, recorded directly against an account.
- **DirectIncome** — Income received directly, not via an invoice, recorded against an account.
- **Invoice** — A sales invoice issued to a customer representing money owed to the company.
- **InvoiceLineItem** — A line item within an Invoice describing a product or service.
- **Payment** — A customer payment applied against one or more Invoices.
- **PurchaseOrder** — A formal order placed with a supplier before a Bill is received.
- **Refund** — A reversal of a payment, either to a customer or from a supplier.
- **SalesOrder** — A customer's order for goods or services before an Invoice is raised.
- **Transfer** — A movement of funds between two accounts within the accounting system.

### Accounting — Master Data

- **Customer** — A person or organization that purchases goods or services from the company.
- **Supplier** — A person or organization that provides goods or services to the company.
- **Item** — A product or service that can appear on invoices, bills, or orders.
- **TaxRate** — A tax code and rate used in accounting transactions.
- **TrackingCategory** — A dimension used to categorize transactions for reporting purposes.

### Accounting — Journals

- **Journal** — A named journal used to group journal entries in accounting software.
- **JournalEntry** — A double-entry bookkeeping record posted to one or more accounts.

### Accounting — Reports

- **BalanceSheet** — A point-in-time financial statement showing assets, liabilities, and equity.
- **Balance** — A monetary value with currency and period context used within financial reports.
- **ProfitAndLoss** — A period financial statement showing income, cost of sales, expenses, and net profit.
- **CashFlow** — A cash flow statement detailing operating, investing, and financing cash movements.
- **Report** — A generic financial report object, wrapping any standardized Codat financial statement.

### Banking

- **BankAccount** — A bank account linked to a company through a banking data connection.
- **BankTransaction** — A transaction record from a linked bank account.
- **BankFeed** — A stream configuration pushing bank transactions into accounting software.

### Commerce

- **CommerceCustomer** — A customer record from a commerce platform such as Shopify or Stripe.
- **Order** — A sales order or transaction record from a commerce platform.
- **Product** — A product listed for sale on a commerce platform.
- **ProductVariant** — A variant of a Product (e.g., size, color) on a commerce platform.
- **Location** — A physical or virtual location associated with a commerce merchant.
- **Dispute** — A chargeback or payment dispute raised on a commerce platform.
- **PaymentLink** — A hosted payment link used to collect payments in a commerce context.
- **CommercePayment** — A payment transaction recorded on a commerce platform.
- **CommerceReport** — A summary or analytics report generated from commerce platform data.

### Lending

- **FinancialProfile** — An aggregated credit profile derived from accounting, banking, and commerce data.
- **AccountsReceivable** — An aging summary of outstanding customer invoices.
- **AccountsPayable** — An aging summary of outstanding supplier bills.
- **EnhancedInvoice** — An invoice enriched with categorization and credit scoring signals.
- **EnhancedCashFlow** — A cash flow statement enhanced with categorized transaction data.
- **LoanTransaction** — A loan draw-down or repayment recorded in accounting software.

### Expenses

- **Expense** — A categorized expense transaction synced from a corporate card or expense platform.
- **ExpenseTransaction** — An individual line item within an Expense record.
- **Attachment** — A receipt or document file attached to an expense or transaction record.

### Payroll

- **PayrollJournalEntry** — A journal entry created from payroll data to be posted to accounting software.
- **Employee** — An employee record used in payroll journal mapping.

## Queries

- `company(id: ID!)` — Fetch a single company by ID.
- `companies(page: Int, pageSize: Int)` — List all companies with pagination.
- `connection(companyId: ID!, connectionId: ID!)` — Fetch a data connection for a company.
- `connections(companyId: ID!)` — List all connections for a company.
- `integrations(page: Int, pageSize: Int)` — List available integrations.
- `pullOperation(companyId: ID!, datasetId: ID!)` — Get status of a pull operation.
- `dataStatus(companyId: ID!, connectionId: ID!)` — Get sync status for all data types.
- `accountingAccounts(companyId: ID!, connectionId: ID!)` — List chart-of-accounts entries.
- `bills(companyId: ID!, connectionId: ID!)` — List bills for a company.
- `invoices(companyId: ID!, connectionId: ID!)` — List invoices for a company.
- `customers(companyId: ID!, connectionId: ID!)` — List customers.
- `suppliers(companyId: ID!, connectionId: ID!)` — List suppliers.
- `bankAccounts(companyId: ID!, connectionId: ID!)` — List linked bank accounts.
- `bankTransactions(companyId: ID!, connectionId: ID!, bankAccountId: ID!)` — List bank transactions.
- `balanceSheet(companyId: ID!, connectionId: ID!, date: String!)` — Fetch balance sheet report.
- `profitAndLoss(companyId: ID!, connectionId: ID!, periodLength: Int!, periodsToCompare: Int!)` — Fetch P&L report.
- `cashFlow(companyId: ID!, connectionId: ID!)` — Fetch cash flow statement.
- `orders(companyId: ID!, connectionId: ID!)` — List commerce orders.
- `products(companyId: ID!, connectionId: ID!)` — List commerce products.
- `expenses(companyId: ID!, connectionId: ID!)` — List expense transactions.

## Mutations

- `createCompany(name: String!, description: String)` — Register a new company in Codat.
- `deleteCompany(id: ID!)` — Remove a company and all its data connections.
- `createConnection(companyId: ID!, platformKey: String!)` — Create a new data connection.
- `deleteConnection(companyId: ID!, connectionId: ID!)` — Remove a data connection.
- `queuePullOperation(companyId: ID!, connectionId: ID!, dataType: String!)` — Trigger a data pull.
- `createWebhook(url: String!, type: String!)` — Register a webhook endpoint.
- `deleteWebhook(id: ID!)` — Remove a webhook registration.
- `createBillPayment(companyId: ID!, connectionId: ID!, input: BillPaymentInput!)` — Post a bill payment.
- `createExpense(companyId: ID!, connectionId: ID!, input: ExpenseInput!)` — Sync an expense record.
- `createJournalEntry(companyId: ID!, connectionId: ID!, input: JournalEntryInput!)` — Post a journal entry.
- `createBankFeed(companyId: ID!, connectionId: ID!, input: BankFeedInput!)` — Configure a bank feed.
