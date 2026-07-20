---
name: Look up Australian Military Bank banking products
description: >-
  Browse and inspect Australian Military Bank's retail banking product
  catalogue via the public, unauthenticated CDR Product Reference Data API.
  Use to list products (optionally by category) and fetch full product detail
  including fees, eligibility, and deposit/lending rates.
api: openapi/australian-military-bank-cds-banking-products-openapi.yml
base_url: https://public.open.australianmilitarybank.com.au/cds-au/v1
operations:
  - listBankingProducts
  - getBankingProductDetail
---

# Look up Australian Military Bank banking products

This API is **public and unauthenticated** — no API key or token. It is the
Consumer Data Right (CDR) Product Reference Data surface built to the DSB
Consumer Data Standards.

## Rules (always)

- Send the version header `x-v: 3` on every request. Omitting or sending an
  unsupported version returns HTTP `406` (`urn:au-cds:error:cds-all:Header/InvalidVersion`).
- Errors come back as `{ "errors": [ { code, title, detail, meta } ] }` where
  `code` is a CDR error URN — this is the CDS format, not RFC 9457.
- Lists are paginated with `page` (1-based) and `page-size`; read
  `meta.totalRecords` / `meta.totalPages` and follow `links.next`.
- Optionally send `x-fapi-interaction-id` (a UUID) for request correlation.

## Steps

1. **List products** — call `listBankingProducts`
   (`GET /banking/products`). Optionally filter with `product-category`
   (e.g. `TRANS_AND_SAVINGS_ACCOUNTS`, `RESIDENTIAL_MORTGAGES`, `PERS_LOANS`,
   `TERM_DEPOSITS`, `CRED_AND_CHRG_CARDS`) and paginate with `page`/`page-size`.
   Each item carries `productId`, `name`, `productCategory`, `brand`,
   `description`, and effective dates.

2. **Get product detail** — for a `productId` of interest, call
   `getBankingProductDetail` (`GET /banking/products/{productId}`) to retrieve
   the full record: `features`, `constraints`, `eligibility`, `fees`
   (with `discounts`), `depositRates`/`lendingRates` (with `tiers`),
   `bundles`, and `additionalInformation`.

3. **Handle errors** — on `404` the `productId` is unknown; on `400`/`422`
   check the offending field named in `errors[].detail`; on `406` correct the
   `x-v` header.

## Notes

- Account, balance, transaction, direct-debit, scheduled-payment, and payee
  operations in the OpenAPI are **not** callable here — they require CDR
  accreditation and the authenticated FAPI/OIDC data-holder flow.
- See `conventions/australian-military-bank-conventions.yml` and
  `errors/australian-military-bank-problem-types.yml` for full semantics.
