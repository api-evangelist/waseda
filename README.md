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

Waseda University is a large private research university in Shinjuku, Tokyo, founded in 1882. This
repository catalogs Waseda's public, machine-readable footprint as an [APIs.json](https://apisjson.org)
profile, under the API Evangelist **university pipeline** — which settles *who operates* each surface
before saving anything, because a university is a federation of buyers and most of what appears under
its name is a vendor's contract.

Waseda operates no developer portal, publishes no OpenAPI, and has no official GitHub organization.
It is not, however, an empty profile: three genuinely institution-operated machine-readable surfaces
sit under Waseda's own domains and answer anonymous or structured calls.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/waseda/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=waseda-api-evangelist&utm_content=repo

## Type

University / Private Research University · Index / Provider / 1st-Party

## Tags

University, Higher Education, Education, Japan, Asia, Private Research University, Research, Library,
Open Access, Cultural Heritage, Digital Archives, IIIF, Identity Federation, Learning Management,
Research Repository

## Surfaces, by operator

Every entry carries an `x-operator`. `method:` says how we came to hold an artifact; `x-operator:`
says who runs the thing it describes.

### institution — Waseda's own

- **Waseda IIIF Presentation API** — `https://iiif.archive.waseda.jp/iiif/manifest` · IIIF
  Presentation 2.1 `sc:Manifest` documents for the Kotenseki Sogo Database (古典籍総合データベース) and the
  Waseda Cultural Resources Database (文化資源データベース). Anonymous, `application/json`, attribution
  "早稲田大学図書館 (Waseda University Library)".
- **Waseda IIIF Image API** — `https://iiif.archive.waseda.jp/iiif/image` · Image API 2.0 compliance
  level 1, 256×256 tiles, `application/ld+json`.
- **Waseda Identity Provider (Shibboleth SAML 2.0)** — `https://iaidp.ia.waseda.jp/idp/shibboleth` ·
  live metadata, `shibmd:Scope waseda.jp`, SAML2 Redirect / POST / POST-SimpleSign SSO and SLO.
- **Waseda Moodle — LTI 1.3 / LTI Advantage platform** — `https://wsdmoodle.waseda.jp/mod/lti` ·
  JWKS keyset (200), OAuth 2.0 client-credentials token endpoint (400 `invalid_request`), LTI services
  endpoint (405), OIDC login endpoint (200).
- **Waseda Moodle Web Services (REST)** — `https://wsdmoodle.waseda.jp/webservice/rest/server.php` ·
  token-gated. Returns **HTTP 200 with an `invalidtoken` fault in the body** — a status-code-only
  check would misread this as an open API.

### federation

- **GakuNin (学術認証フェデレーション)** — Waseda's IdP entityID is registered in NII's operational
  federation aggregate and reaches eduGAIN through it. A federation is shared by definition; the IdP
  inside it is Waseda's.

### tenant — Waseda's data, someone else's contract

- **Waseda University Repository (OAI-PMH 2.0)** — `https://waseda.repo.nii.ac.jp/oai` · seven
  metadata formats including JPCOAR 2.0, DDI and IEEE LOM. The collection and the admin contact
  (`repository@list.waseda.jp`) are Waseda's; the host and the WEKO3 software are NII's JAIRO Cloud.
- **WINE Library Discovery** — Ex Libris Primo VE tenancy, institution code `81SOKEI_WUNI`. Alma SRU
  is **not** enabled (404 `SERVICE_NOT_FOUND`), so the previously recorded "Primo/SRU interfaces
  exist" claim is unverifiable and has been re-stated as such.

### registry — memberships, not contracts

- **ROR** — https://ror.org/00ntfnx83 (established 1882; GRID `grid.5290.e`, ISNI `0000 0004 1936 9975`,
  Wikidata `Q274486`).
- **Crossref Open Funder Registry** — `501100004423`, 1,458 works. Waseda is in the Funder Registry
  only; a Crossref *members* query returns zero, so it is not a DOI-depositing member.
- **DataCite** — no account. `api.datacite.org/providers?query=Waseda` returns `meta.total: 0`.

## Domain standard conformance (Kin Score `education` regime)

Reward-only, established by live credential-free probe — see
[conformance/waseda-conformance.yml](conformance/waseda-conformance.yml).

| Standard | Status | Operator |
|---|---|---|
| `lti` | conformant (1.3 / Advantage) | institution |
| `saml` | conformant (2.0) | institution |
| `shibboleth` | conformant | institution |
| `oai-pmh` | conformant (2.0) | tenant |
| `crossref` | registered (Funder Registry) | registry |
| `scim`, `oneroster`, `ed-fi`, `caliper`, `qti`, `orcid`, `datacite` | not found | — |

Also evidenced outside the regime list: IIIF Image API 2.0, IIIF Presentation API 2.1, OAuth 2.0
client-credentials, RFC 7517 JWKS, ROR.

## Artifacts

- [conformance/waseda-conformance.yml](conformance/waseda-conformance.yml) — `method: probed`
- [authentication/waseda-authentication.yml](authentication/waseda-authentication.yml) — `method: probed`
- [examples/waseda-examples.yml](examples/waseda-examples.yml) — `method: probed`, verbatim captures
- [plans/waseda-plans-pricing.yml](plans/waseda-plans-pricing.yml) ·
  [rate-limits/waseda-rate-limits.yml](rate-limits/waseda-rate-limits.yml) ·
  [finops/waseda-finops.yml](finops/waseda-finops.yml) ·
  [security/waseda-domain-security.yml](security/waseda-domain-security.yml)

There is **no `openapi/` directory** and that is deliberate. Waseda publishes no OpenAPI. The IIIF,
LTI, SAML and OAI-PMH surfaces are deployments of open standards whose contracts belong to those
standards bodies, not to Waseda — generating a spec from them would credit Waseda with engineering it
did not do, which is exactly the failure this pipeline exists to prevent.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.waseda.jp/top/en/
- Privacy Policy: https://www.waseda.jp/top/en/privacy-policy
- Support / IT Service Portal: https://support.waseda.jp/it/s/
- Identity Federation: https://iaidp.ia.waseda.jp/idp/shibboleth
- Research Repository: https://waseda.repo.nii.ac.jp/
- Library Catalog (WINE): https://waseda.primo.exlibrisgroup.com/discovery/search?vid=81SOKEI_WUNI:WINE
- Course Catalog (syllabus search): https://www.wsl.waseda.jp/syllabus/JAA101.php
- Open Data / Cultural Resources Database: https://archive.waseda.jp/archive/
- AI Policy: https://www.waseda.jp/top/news/89507?lng=en
- Image use terms: https://www.waseda.jp/library/user/using-images/
- LinkedIn: https://www.linkedin.com/school/wasedauniversity/

## Notes

- **No official GitHub organization.** `github.com/wasedatime` is an unaffiliated student project; its
  backend `api.wasedatime.com` returns 403 with no public documentation and no evidence of
  institutional endorsement. The previous `GitHub` pointer claiming it has been removed, because a
  student surface on a non-institution domain is a tenant relationship at best and this one is not
  even that. `nlp-waseda` and `ogata-lab` are individual lab organizations, not the university's.
- **`waseda.repo.nii.ac.jp` bot-blocks browsers.** The whole host returns 406 Not Acceptable to a
  desktop-browser User-Agent and 200 to a plain client. That is a content-negotiation quirk on NII's
  nginx, not an outage — a naive liveness check will report it dead.
- **`www.waseda.jp` returns 403, not 404, for `/robots.txt`, `/llms.txt` and
  `/.well-known/security.txt`.** Those are recorded as *unreadable*, not as confirmed absent.
- **`researchers.waseda.jp` timed out** at 60 seconds on 2026-09-01 and is not emitted as a pointer.
  The live researcher database is `https://w-rdb.waseda.jp/` (institution-operated, HTML only).
- No fabrication: every endpoint above was probed live on 2026-09-01 and every status code is recorded
  in [review.yml](review.yml) and in the `x-coverage` block of `apis.yml`.

## Maintainers

- Kin Lane — kin@apievangelist.com
