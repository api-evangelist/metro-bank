# Metro Bank (metro-bank)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Metro Bank is a UK retail and commercial bank founded in 2010 as the first new high-street bank to open in Britain in over 150 years, headquartered in London and listed on the London Stock Exchange (LSE: MTRO). It is a public limited company (not a mutual or building society), authorised by the Prudential Regulation Authority and regulated by the Financial Conduct Authority and the PRA. As an FCA-authorised account servicing payment service provider (ASPSP) under PSD2, Metro Bank participates in UK Open Banking - without being one of the nine CMA-mandated banks (the CMA9) - and operates a public developer portal, built on Google Apigee, publishing APIs aligned to the Open Banking Implementation Entity (OBIE) standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/apis.yml)

## Tags

- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

### Metro Bank Open Data API

Public, unauthenticated OBIE Open Data reference API exposing ATM locations, branch ("store") locations, personal and business current account products, unsecured SME loans, and commercial credit card products, conformant to the UK Open Banking Open Data API standard.

- **Human URL:** [https://developer.metrobankonline.co.uk/Overview](https://developer.metrobankonline.co.uk/Overview)
- **Base URL:** `https://api.metrobankonline.co.uk/open-banking/v2.3`

#### Tags

- Open Data
- ATMs
- Branches
- Products

#### Properties

- [OpenAPI](openapi/obie-open-data-api-standard-v1.3-swagger.json) — shared OBIE Open Data API standard (v1.3), not a Metro-proprietary contract
- [Documentation](https://developer.metrobankonline.co.uk/Overview)
- [API Reference](https://openbankinguk.github.io/opendata-api-docs-pub/v2.4.0/)

### Metro Bank Account and Transaction Information API

OBIE Read/Write Account Information Service (AIS) API providing consented access to account details, balances, transactions, beneficiaries, standing orders, direct debits, and statements. FAPI-secured with OAuth2/OIDC, mutual TLS, and PSD2 strong customer authentication.

- **Human URL:** [https://developer.metrobankonline.co.uk/Overview](https://developer.metrobankonline.co.uk/Overview)
- **Base URL:** `https://api.metrobankonline.co.uk/open-banking/v3.1/aisp`

#### Tags

- Account Information
- AIS
- Transactions

### Metro Bank Payment Initiation API

OBIE Read/Write Payment Initiation Service (PIS) API for initiating domestic and scheduled payments, standing orders, and file payments on behalf of a consenting customer. FAPI-secured with OAuth2/OIDC, mutual TLS, and PSD2 strong customer authentication.

- **Human URL:** [https://developer.metrobankonline.co.uk/Overview](https://developer.metrobankonline.co.uk/Overview)
- **Base URL:** `https://api.metrobankonline.co.uk/open-banking/v3.1/pisp`

#### Tags

- Payment Initiation
- PIS
- Payments

### Metro Bank Confirmation of Funds API

OBIE Read/Write Confirmation of Funds (CBPII) API allowing a card-based payment instrument issuer to confirm whether sufficient funds are available on a customer account. FAPI-secured with OAuth2/OIDC, mutual TLS, and PSD2 strong customer authentication.

- **Human URL:** [https://developer.metrobankonline.co.uk/Overview](https://developer.metrobankonline.co.uk/Overview)
- **Base URL:** `https://api.metrobankonline.co.uk/open-banking/v3.1/cbpii`

#### Tags

- Confirmation of Funds
- CBPII

### Metro Bank FCA Account Metrics API

API publishing Metro Bank's FCA service-quality and account metrics data (management information required under UK regulatory reporting), documented in the Metro Bank developer portal.

- **Human URL:** [https://developer.metrobankonline.co.uk/FCA-Account-Metrics-API](https://developer.metrobankonline.co.uk/FCA-Account-Metrics-API)
- **Base URL:** `https://api.metrobankonline.co.uk/open-banking/v3.1`

#### Tags

- FCA
- Account Metrics
- Reporting

## Common Properties

- [Website](https://www.metrobankonline.co.uk/)
- [Developer Portal](https://developer.metrobankonline.co.uk/)
- [Documentation](https://developer.metrobankonline.co.uk/Overview)
- [LinkedIn](https://www.linkedin.com/company/metro-bank)
- [Blog](https://www.metrobankonline.co.uk/about-us/press-releases/)
- [Support](https://www.metrobankonline.co.uk/help-and-support/)
- [Privacy Policy](https://www.metrobankonline.co.uk/privacy/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
