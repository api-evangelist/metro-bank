# Metro Bank (metro-bank)

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
