# Aerones

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

Aerones is a Latvian robotics company that inspects, cleans, coats and repairs wind
turbine blades with cable-suspended robots and autonomous drones, onshore and offshore,
for owners and OEMs including NextEra, GE, Vestas, Enel and Siemens Gamesa.

## What was found

The software side of Aerones is the **Operations Hub**, the Django Ninja backend behind
`portal.aerones.com`. It publishes a machine-readable contract anonymously:

| Surface | Where | Size |
|---|---|---|
| OpenAPI 3.1.0 | `https://operations.aerones.com/api/openapi.json` | 760 paths, 1,114 operations, 1,377 schemas |
| Swagger UI | `https://operations.aerones.com/api/docs` | renders the above |
| GraphQL SDL | `https://operations.aerones.com/api/graphql-schema` | 1,524 types, 339 queries, 325 mutations, 4 subscriptions |
| GraphQL endpoint | `https://operations.aerones.com/graphql` | introspection answers anonymously |
| OIDC discovery | `https://sso.aerones.com/realms/aerones/.well-known/openid-configuration` | Keycloak, client `operations-hub` |

The **descriptions** are public. The **data** is not — 1,089 of the 1,114 operations
require a bearer token from the Keycloak realm above or the `opshub_prod_sessionid`
session cookie, and no data endpoint was called in building this profile.

## What is absent

No developer programme, no SDKs in any registry, no GitHub organization, no MCP server,
no agent card, no `security.txt`, no status page, no changelog, no published rate limits,
no API pricing, and no deprecation policy — though 33 operations are flagged
`deprecated` in the contract itself. Errors use a bespoke `{code, message}` envelope
rather than RFC 9457, and the write surface has no `Idempotency-Key`: seven operations
declare idempotent semantics in prose and roughly 480 others have no replay protection.

Certifications published: ISO 9001, ISO 14001, ISO 45001 and GWO training standards
(via KIWA and TÜV NORD). No information-security certification (SOC 2, ISO 27001) is
published and no trust center exists.

- https://aerones.com/
- https://operations.aerones.com/api/docs
- https://portal.aerones.com/
