# Aceable

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
