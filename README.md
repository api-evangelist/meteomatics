# Meteomatics (meteomatics)

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
