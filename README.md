# Aceable

Aceable (Aceable Brands) is an Austin, Texas mobile-first online education company founded in 2013 that builds state-accredited licensing and continuing-education courses across four brands:

- **Aceable** — drivers ed, defensive driving and traffic school in 40+ US states — https://www.aceable.com/
- **Aceable Agent** — real estate pre-license, post-license and CE in 16 states, plus PrepAgent exam prep in all 50 — https://www.aceableagent.com/
- **Aceable Insurance** — Property & Casualty and Life & Health pre-license in 13 states, CE in CA/IL/TX — https://insurance.aceable.com/
- **Aceable Mortgage** — NMLS-approved MLO pre-license and CE in 7 states plus the required 20-hour national component (NMLS Provider ID 1400102) — https://mortgage.aceable.com/

More than 20 million students have been licensed through Aceable, at roughly 1.5 million per year. A B2B partner program (affiliate and bulk-buy) serves driving schools, school districts, brokerages, carriers and mortgage employers — https://partnerships.aceable.com/

## API surface

**Aceable publishes no public developer API.** As of 2026-08-02 no OpenAPI/Swagger, GraphQL schema, AsyncAPI, MCP server, A2A agent card or developer portal was found on any Aceable host. A private platform API is observable at `https://api.aceable.com` (Express on Heroku), but every probed path returns HTTP 401 `{"errorList":[{"message":"Cannot Authorize Application ID","code":40100}]}` — an application-gated first-party backend for the Aceable web and mobile apps, not a published API product.

The GitHub organization https://github.com/aceable (named "XGRIT (Platform)") holds seven public repositories — CI/CD actions, an Angular/React interop library and boilerplates — and no client SDKs.

## What is captured here

| Artifact | What it holds |
|---|---|
| `llms/` | The five verbatim `llms.txt` files Aceable publishes, one per brand host |
| `well-known/` | Full `/.well-known/*` probe results across every host (zero documents found) |
| `security/` | TLS/HSTS/DNSSEC/CAA/SPF/DMARC probe across seven hosts and two registrable domains |
| `conformance/` | Published state and federal course accreditations (TDLR, CA DMV, TREC, NMLS, state insurance departments, Perkins V) plus API-standard applicability |
