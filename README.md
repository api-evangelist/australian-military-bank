# Australian Military Bank (australian-military-bank)

Australian Military Bank Ltd (ABN 48 087 649 741, AFSL/Australian Credit Licence 237988, BSB 642170) is a customer-owned mutual authorised deposit-taking institution (ADI) that has served the Australian Defence Force community, veterans, and their families since 1959. As an active ADI it participates in Australia's Consumer Data Right (CDR) open banking regime, and its only public, unauthenticated API surface is the mandated Product Reference Data (PRD) API built to the Data Standards Body (DSB) Consumer Data Standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/apis.yml)

## Tags

- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Defence

## Timestamps

- **Created:** 2026-07-20
- **Modified:** 2026-07-20

## APIs

### Australian Military Bank CDR Product Reference Data API

Public, unauthenticated Consumer Data Right (CDR) Product Reference Data API exposing Australian Military Bank's retail banking product catalogue. Confirmed live at `https://public.open.australianmilitarybank.com.au/cds-au/v1/banking/products` (HTTP 200, `x-v: 3`, 39 products across 2 pages). Conforms to the DSB Consumer Data Standards Banking API and provides `GET /banking/products` (list, filterable/paginated) and `GET /banking/products/{productId}` (product detail) with no authentication.

- **Human URL:** [https://www.australianmilitarybank.com.au/consumer-data-right](https://www.australianmilitarybank.com.au/consumer-data-right)
- **Base URL:** `https://public.open.australianmilitarybank.com.au/cds-au/v1`

#### Tags

- CDR
- Open Banking
- Product Reference Data
- Banking Products
- Public

#### Properties

- [Documentation](https://www.australianmilitarybank.com.au/consumer-data-right)
- [API Reference](https://consumerdatastandardsaustralia.github.io/standards/#get-products)
- [OpenAPI](openapi/australian-military-bank-cds-banking-products-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Website](https://www.australianmilitarybank.com.au/)
- [Developer Portal](https://www.australianmilitarybank.com.au/consumer-data-right)
- [LinkedIn](https://www.linkedin.com/company/australian-military-bank)
- [Terms of Service](https://www.australianmilitarybank.com.au/disclosuredocuments)
- [Privacy Policy](https://www.australianmilitarybank.com.au/privacy)
- [Security](https://www.australianmilitarybank.com.au/securityhub)
- [Support](https://www.australianmilitarybank.com.au/contact)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
