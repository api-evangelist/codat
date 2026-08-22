# Codat (codat)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Codat is a unified API platform focused on SMB financial data, connecting to 30+ accounting, ERP, banking, and payment platforms.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Unified_API

## Timestamps

- **Created:** 2026-03-03
- **Modified:** 2026-05-19

## APIs

### Codat Platform API

The Codat Platform API provides core functionality used across all Codat solutions, including programmatic creation and management of companies, data connections, and configuration of integrations with accounting, banking, and commerce platforms.

- **Human URL:** [https://docs.codat.io/using-the-api/overview](https://docs.codat.io/using-the-api/overview)

#### Tags

- Companies
- Connections
- Platform
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/using-the-api/overview)
- [API Reference](https://docs.codat.io/platform-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [OpenAPI](openapi/codat-platform-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Codat Lending API

The Codat Lending API enables digital lenders, neobanks, and corporate card providers to make smarter credit decisions on small businesses by aggregating and analyzing standardized financial data from accounting, banking, and commerce platforms to assess SMB creditworthiness.

- **Human URL:** [https://docs.codat.io/lending/overview](https://docs.codat.io/lending/overview)

#### Tags

- Credit
- Financial Data
- Lending
- Underwriting
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/lending/overview)
- [API Reference](https://docs.codat.io/lending-api)
- [OpenAPI](openapi/codat-lending-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Open A P I  Source](https://github.com/codatio/oas)

### Codat Bank Feeds API

The Codat Bank Feeds API enables banks, neobanks, corporate card issuers, and payment providers to set up automatic bank feeds from their applications to supported accounting software, simplifying the deployment of bank statement synchronization into SMB accounting platforms through a single standardized integration.

- **Human URL:** [https://docs.codat.io/bank-feeds/overview](https://docs.codat.io/bank-feeds/overview)

#### Tags

- Accounting
- Bank Feeds
- Reconciliation
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/bank-feeds/overview)
- [OpenAPI](openapi/codat-bank-feeds-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://docs.codat.io/bank-feeds-api)
- [Open A P I  Source](https://github.com/codatio/oas)

### Codat Sync for Expenses API

The Codat Sync for Expenses API enables corporate card and expense management platforms to provide high-quality integrations with multiple accounting platforms, synchronizing categorized expense data including receipts, general ledger mappings, and tracking categories into SMB accounting software through a standardized data model.

- **Human URL:** [https://docs.codat.io/expenses/overview](https://docs.codat.io/expenses/overview)

#### Tags

- Accounting Sync
- Corporate Cards
- Expenses
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/expenses/overview)
- [API Reference](https://docs.codat.io/sync-for-expenses-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Codat Bill Pay API

The Codat Bill Pay API (Sync for Payables) enables neobanks, expense management providers, and B2B payment platforms to automate customers' accounts payable workflows, providing a standardized data model to sync bills and bill payments with all major accounting software in real time.

- **Human URL:** [https://docs.codat.io/payables/overview](https://docs.codat.io/payables/overview)

#### Tags

- Accounts Payable
- Bill Pay
- Payables
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/payables/overview)
- [API Reference](https://docs.codat.io/sync-for-payables-v2-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Codat Spend Insights API

The Codat Spend Insights API enables banks and commercial card issuers to access clients' accounts payable data from their ERP or accounting software within minutes, providing insights on spend and supplier activity to identify suppliers eligible for virtual card programs and grow commercial card volume in B2B payments.

- **Human URL:** [https://docs.codat.io/spend-insights/overview](https://docs.codat.io/spend-insights/overview)

#### Tags

- Accounts Payable
- Spend Insights
- Unified_API
- Virtual Cards

#### Properties

- [Documentation](https://docs.codat.io/spend-insights/overview)
- [API Reference](https://docs.codat.io/spend-insights-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Codat Sync for Commerce API

The Codat Sync for Commerce API automatically replicates and reconciles sales data from merchant point-of-sale, payments, and eCommerce systems into their accounting software, transforming raw sales and payments data into detailed sales invoices for automated accounting reconciliation.

- **Human URL:** [https://docs.codat.io/commerce/overview](https://docs.codat.io/commerce/overview)

#### Tags

- Commerce
- Point of Sale
- Reconciliation
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/commerce/overview)
- [API Reference](https://docs.codat.io/sync-for-commerce-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Codat Sync for Payroll API

The Codat Sync for Payroll API enables HR, payroll, and vertical SaaS platforms to integrate their customers' payroll data into accounting software and support its reconciliation, providing a standardized data model to create and manage accounts, journal entries, and tracking categories across all supported accounting and ERP packages.

- **Human URL:** [https://docs.codat.io/payroll/overview](https://docs.codat.io/payroll/overview)

#### Tags

- Accounting Sync
- HR
- Payroll
- Unified_API

#### Properties

- [Documentation](https://docs.codat.io/payroll/overview)
- [API Reference](https://docs.codat.io/sync-for-payroll-api)
- [Open A P I  Source](https://github.com/codatio/oas)
- [Postman Collection](collections/codat-bank-feeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-bank-feeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-lending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-lending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/codat-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/codat-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/codat-limited)
- [Portal](https://app.codat.io/)
- [Documentation](https://docs.codat.io/)
- [Getting Started](https://docs.codat.io/get-started/first-steps)
- [S D Ks](https://docs.codat.io/get-started/libraries)
- [Open A P I  Source](https://github.com/codatio/oas)
- [GitHub Organization](https://github.com/codatio)
- [Blog](https://codat.io/blog/)
- [Changelog](https://docs.codat.io/updates)
- [Status Page](https://status.codat.io)
- [Sign Up](https://codat.io/start-building/)
- [About](https://codat.io/about/)
- [Legal](https://legal.codat.io/)
- [Type Script  S D K](https://github.com/codatio/client-sdk-typescript)
- [Python  S D K](https://github.com/codatio/client-sdk-python)
- [C#  S D K](https://github.com/codatio/client-sdk-csharp)
- [Go  S D K](https://github.com/codatio/client-sdk-go)
- [Java  S D K](https://github.com/codatio/client-sdk-java)
- [L L Ms Txt](https://codat.io/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
