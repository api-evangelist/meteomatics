# Meteomatics (meteomatics)

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

Meteomatics is a Swiss weather technology company offering a REST and WebSocket Weather API that provides hyperlocal forecasts, historical weather data back to 1940, climate scenarios to 2100, marine conditions, and environmental parameters at up to 1km native resolution. The API exposes over 1,800 weather parameters across global, regional, oceanic, and AI-based models, supporting point, multi-location, route, and polygon queries with output in JSON, CSV, XML, PNG, GeoTIFF, and NetCDF formats. Authentication is via basic auth over HTTPS or OAuth2 JWT tokens (valid 2 hours), with usage tracked via the user_stats endpoint.

APIs.json: https://raw.githubusercontent.com/api-evangelist/meteomatics/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=meteomatics-api-evangelist&utm_content=repo

## Tags

- Weather
- Forecast
- Climate
- Historical Weather
- Marine
- Environmental Data
- Hyperlocal
- Meteorology
- Time Series
- Geospatial

## APIs

### Meteomatics Weather API

REST API providing access to over 1,800 weather parameters including forecasts, historical data, climate scenarios, marine conditions, and environmental variables at up to 1km resolution globally.

- **Base URL:** https://api.meteomatics.com
- **Documentation:** https://www.meteomatics.com/en/api/
- **Getting Started:** https://www.meteomatics.com/en/api/getting-started/
- **Authentication:** https://www.meteomatics.com/en/api/request/api-requests-oauth-authentification/
- **Tutorials:** https://www.meteomatics.com/en/api/api-tutorials/
- **FAQ:** https://www.meteomatics.com/en/api/faq/

## Plans / Rate Limits / FinOps

- **Plans & Pricing:** [plans/meteomatics-plans-pricing.yml](plans/meteomatics-plans-pricing.yml) — Free 14-day trial (500 req/day, 50 req/min, 10 parallel); paid tiers are custom-quoted based on query volume, resolution, and SLA requirements.
- **Rate Limits:** [rate-limits/meteomatics-rate-limits.yml](rate-limits/meteomatics-rate-limits.yml) — Free trial: 500 req/day, 50 req/min, 10 concurrent. Paid: contract-defined. Monitor via `https://api.meteomatics.com/user_stats_json`.
- **FinOps:** [finops/meteomatics-finops.yml](finops/meteomatics-finops.yml) — Primary cost drivers are query volume, data resolution (1km EURO1k/US1k vs. global), parameter breadth, and SLA tier. Key optimizations: cache responses, batch multi-location queries, consolidate parameters per request, monitor user_stats.

## Timestamps

- **Created:** 2026-06-12
- **Modified:** 2026-06-12

## Common

| Type | URL |
|------|-----|
| Website | https://www.meteomatics.com |
| Documentation | https://www.meteomatics.com/en/api/ |
| GitHub | https://github.com/meteomatics |
| LinkedIn | https://www.linkedin.com/company/meteomatics |
| Blog | https://www.meteomatics.com/en/tech-blog/ |
| Pricing | https://www.meteomatics.com/en/pricing/ |
| Status Page | https://sanes.co |
| X (Twitter) | https://twitter.com/meteomatics |
| Service Level Agreement | https://www.meteomatics.com/en/service-level-agreement/ |

## Maintainers

| Name | Email |
|------|-------|
| Kin Lane | kin@apievangelist.com |
