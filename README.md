# Budget Direct (budget-direct)

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

Budget Direct is one of Australia's largest direct-to-consumer general insurance brands, operated from Toowong, Queensland by Auto & General Services Pty Ltd (ABN 61 003 617 909), with general insurance products issued by Auto & General Insurance Company Limited (ABN 42 111 586 353), an APRA-authorised insurer. The brand sells car, home and contents, motorcycle, travel, pet and life insurance plus roadside assistance direct to Australian consumers online and by phone — life cover underwritten by NobleOak Life Limited, travel cover by Zurich Australian Insurance Limited. Its parent, Auto & General, also white-labels personal lines through distribution partners including Qantas, Coles Insurance, ING and Oceania Insurance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/budget-direct/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/budget-direct/refs/heads/main/apis.yml)

## Tags

- Insurance
- Australia
- Property and Casualty
- Direct to Consumer Insurance
- Motor Insurance
- Home Insurance
- Travel Insurance
- Life Insurance
- Underwriting
- Claims
- Carrier
- No Public API

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None.** Budget Direct publishes no public, self-serve API and no developer portal.

This is the honest finding, not a gap in research. Every conventional developer host and path was probed on 2026-07-25:

| Surface | Result |
| --- | --- |
| `developer.` / `developers.` / `docs.` / `api.` / `apis.` / `partners.` / `portal.` / `broker.` / `sandbox.budgetdirect.com.au` | DNS does not resolve |
| `/developers`, `/developer`, `/api`, `/partners`, `/integrations` | HTTP 404 |
| `/openapi.json`, `/swagger.json`, `/api-docs`, `/graphql` | HTTP 404 (HTML error pages, no specs) |
| `/.well-known/openid-configuration`, `/.well-known/oauth-authorization-server` | HTTP 404 |
| Published sitemap (738 URLs) | No developer, API or integration page |
| `autogeneral.com.au/partners/` | HTTP 200 — commercial partner list, zero technical integration content |

- **ACORD posture:** no ACORD reference found. No mention of ACORD, AL3, ACORD XML, ACORD certified or NGDS on either budgetdirect.com.au or autogeneral.com.au — consistent with a direct-to-consumer carrier that has no agency-management-system channel to feed.
- **Quote / bind / issue / FNOL:** all four exist only as consumer web journeys and a logged-in "existing customers" self-service area. None is exposed as a documented machine interface.
- **Auth model:** none published. The only authentication surface is the consumer customer login.
- **Webhooks / events / AsyncAPI:** none. **Postman:** none. **GraphQL / gRPC:** none.
- **Infrastructure note:** the parent domain carries a first-party Apigee gateway hostname (`api.autogeneral.com.au`, CNAME to `autogeneral-prod.apigee.net`) that the consumer site preconnect-hints. It is undocumented, unreachable anonymously, and not offered as a public API. A separate `docs.autogeneral.com.au` host serves an S3 listing of marketing and compliance PDFs (PDS, FSG, claim forms) — not API documentation.

Australia has the legal machinery for open insurance and no live obligation: the Consumer Data Right that opened banking and energy was designated to extend to general insurance and then deferred. With no forcing function, an APRA-regulated carrier like Budget Direct has no reason to publish an API, and it does not.

## Links

- [Website](https://www.budgetdirect.com.au/)
- [About](https://www.budgetdirect.com.au/about-us.html)
- [Contact](https://www.budgetdirect.com.au/contact-us.html)
- [Code of Practice](https://www.budgetdirect.com.au/about-us/code-of-practice.html)
- [Media Releases](https://www.budgetdirect.com.au/about-us/media-releases.html)
- [LinkedIn](https://au.linkedin.com/company/budget-direct)
- [Parent — Auto & General](https://www.autogeneral.com.au/)
- [Auto & General Partners](https://www.autogeneral.com.au/partners/)
