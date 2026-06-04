# Waseda University (waseda)

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
