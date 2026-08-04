# Waseda University (waseda)

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

Waseda University is a leading private research university in Tokyo, Japan, ranked #181 in the QS World University Rankings 2025. This repository catalogs Waseda's public, machine-readable developer/API footprint as an [APIs.json](https://apisjson.org) profile. Waseda does not operate a dedicated developer portal; its confirmed footprint is centered on scholarly infrastructure — an OAI-PMH institutional repository, an Ex Libris Primo/Alma library discovery service (WINE), and Shibboleth SAML single sign-on.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/waseda/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=waseda-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Library, Open Access, Japan

## APIs

- **Waseda University Repository (OAI-PMH)** — OAI-PMH 2.0 metadata harvesting for the institutional repository (NII WEKO/JAIRO Cloud). Base URL: `https://waseda.repo.nii.ac.jp/oai`. Docs: https://www.openarchives.org/OAI/openarchivesprotocol.html
- **WINE Library Discovery (Ex Libris Primo)** — Library discovery on Ex Libris Primo/Alma (institution code 81SOKEI_WUNI); Primo/SRU APIs exist but are credentialed and not openly documented. Docs: https://waseda-jp.libguides.com/winehelp_en
- **Waseda Identity Provider (Shibboleth SAML SSO)** — Institutional SAML single sign-on. Endpoint: `https://iaidp.ia.waseda.jp/idp/shibboleth`. Docs: https://www.waseda.jp/navi/e/mywaseda/about.html

## Plans

See [plans/waseda-plans-pricing.yml](plans/waseda-plans-pricing.yml).

## Rate Limits

See [rate-limits/waseda-rate-limits.yml](rate-limits/waseda-rate-limits.yml).

## FinOps

See [finops/waseda-finops.yml](finops/waseda-finops.yml).

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.waseda.jp/top/en/
- GitHub (unofficial student org): https://github.com/wasedatime
- LinkedIn: https://www.linkedin.com/school/wasedauniversity/
- Authentication: https://iaidp.ia.waseda.jp/idp/shibboleth

## Notes

All entries reflect a no-fabrication review: only URLs probed live on 2026-06-03 are reported. No dedicated Waseda developer portal or published OpenAPI specifications were found. The OAI-PMH endpoint was verified via a live Identify response. The WINE/Primo and Shibboleth interfaces are real platform capabilities but are not openly documented for general public API consumption. There is no single official Waseda University GitHub organization; only lab and student project orgs (e.g., WasedaTime, nlp-waseda, ogata-lab) exist. The unofficial WasedaTime backend (`api.wasedatime.com`) is reachable but returns 403 and has no public documentation.

## Maintainers

- Kin Lane — kin@apievangelist.com
