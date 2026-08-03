# Australian Military Bank (australian-military-bank)

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
