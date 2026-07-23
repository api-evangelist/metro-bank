---
name: Look up Metro Bank Open Data (branches, ATMs, products)
description: >-
  Query Metro Bank's public OBIE Open Data reference API for branch and ATM
  locations and personal/business account, SME loan, and commercial credit card
  product terms. No authentication required.
api: openapi/obie-open-data-api-standard-v1.3-swagger.json
operations:
  - GET /branches
  - GET /atms
  - GET /personal-current-accounts
  - GET /business-current-accounts
  - GET /unsecured-sme-loans
  - GET /commercial-credit-cards
---

# Look up Metro Bank Open Data

Metro Bank publishes an OBIE Open Data reference API (v2.3 on the live host) that
is **public and unauthenticated**. Use it to retrieve branch/ATM locations and
published product terms. Do not use it for account, balance, transaction, or
payment data - that lives on the FAPI-secured Read/Write APIs (see
`authentication/metro-bank-authentication.yml`).

## Base
- Host: `https://api.metrobankonline.co.uk/open-banking/v2.3`
- No auth. HTTPS only. Accept `application/prs.openbanking.opendata.v1.3+json`.

## Steps
1. Choose the collection:
   - Locations: `GET /branches`, `GET /atms`
   - Products: `GET /personal-current-accounts`, `GET /business-current-accounts`,
     `GET /unsecured-sme-loans`, `GET /commercial-credit-cards`
2. Send a plain `GET`. Optionally send `If-Modified-Since` / `If-None-Match` to
   get `304 Not Modified` when data is unchanged (see
   `conventions/metro-bank-conventions.yml`).
3. Read the response envelope:
   - `meta.LastUpdated`, `meta.TotalResults`, `meta.Agreement`
   - `data[]` - the array of the requested entity.
4. Handle errors by HTTP status (`errors/metro-bank-problem-types.yml`):
   `429` means slow down and retry with backoff; `503` is transient - retry later;
   `400`/`500` are terminal for that request.

## Notes
- `GET` calls are idempotent and cacheable; honour `ETag`/`Last-Modified`.
- This is reference data only - never treat it as customer or account data.
