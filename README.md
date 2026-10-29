# Conviva

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

Conviva is the streaming-media and digital-experience analytics company behind Experience-Centric Operations (ECO) — a real-time, full-census operational data platform that stitches client-side telemetry from its Sensor SDKs into stateful, per-viewer experience analytics for video streamers, broadcasters and app publishers. Its Pulse portal is fronted by a public REST surface at api.conviva.com covering Metrics V3, Sessions V3, AI Alerts, Bulk Filters, Precision Policy, PII Opt-Out and Validation Timeline, plus Conviva Connect session-summary data feeds (S3/GCS/Snowflake/BigQuery/SFTP), alert webhooks, and two hosted OAuth-protected Model Context Protocol servers (mcp.conviva.com for VSI/DPI metrics, alerts and sessions; dpi-mcp.conviva.com for Context Center, Nexa analysis, metric query and session replay). Conviva publishes a large first-party SDK estate — JavaScript/npm, Android/Maven, iOS/CocoaPods+SPM, React Native, Node and Python agent SDKs — and a Claude plugin marketplace carrying three provider-authored Agent Skills for its DPI MCP server. Authentication across the REST surface is HTTP Basic with a client-id/client-secret API key pair generated in Pulse API Management.

**Areas:** Analytics · Streaming · Video · Observability · Monitoring · Media · Quality of Experience · Real-Time · Telemetry · Agents · MCP · Company

## Conviva on APIs.io

Everything profiled for Conviva is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/conviva/](https://apis.io/providers/conviva/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Conviva Metrics V3 API](https://apis.io/apis/conviva/metrics-v3/) — Programmatic access to historical and real-time Conviva experience metrics by metric name, with optional group-by dimensions, saved or dimensional filters,…
- [Conviva Sessions V3 API](https://apis.io/apis/conviva/sessions-v3/) — Session-level detail for content and ad sessions, including per-viewer session diagnostics, network_info with IPv4/IPv6, and summary metrics. Endpoints…
- [Conviva AI Alerts API](https://apis.io/apis/conviva/ai-alerts/) — Retrieval of AI-driven content and ad alerts, alert diagnostics and impacted-session detail, filterable by time range and severity. Endpoints are…
- [Conviva Bulk Filters API](https://apis.io/apis/conviva/bulk-filters/) — Bulk create, retrieve, update and delete of saved Conviva filters so large filter sets can be managed programmatically. Each call processes a maximum of 100…
- [Conviva Precision Policy API](https://apis.io/apis/conviva/precision-policy/) — Programmatic control over Conviva Precision policies — retrieve policy definitions and their filters and resource shares, activate policies, and reorder…
- [Conviva PII Opt-Out API](https://apis.io/apis/conviva/pii-opt-out/) — Privacy-request surface for marking viewer identifiers for opt-out and deletion of Personally Identifiable Information, plus retrieval of opt-out request…
- [Conviva Validation Timeline API v2](https://apis.io/apis/conviva/validation-timeline-v2/) — Session validation timeline data for QA and sensor-integration testing, queried by viewer_id and/or session_id, used to verify that a Conviva Sensor…
- [Conviva MCP Server](https://apis.io/apis/conviva/mcp/) — Hosted Model Context Protocol server exposing Conviva VSI and DPI data to agents across five sub-services — /vsi/metrics, /vsi/ai-alerts, /vsi/sessions,…
- [Conviva DPI MCP Server](https://apis.io/apis/conviva/dpi-mcp/) — Hosted Model Context Protocol server for the Conviva Digital Intelligence Platform, exposing /insights, /nexa, /context-center, /session-replay and…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Conviva Alerts Webhooks](https://apis.io/asyncapis/conviva/conviva-alerts-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [conviva-mcp.yml](https://apis.io/servers/conviva/conviva-mcp-yml/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Conviva Authentication](https://apis.io/security/conviva/conviva-authentication/)
- [Conviva Domain Security](https://apis.io/security/conviva/conviva-domain-security/)
- [Conviva Trust Center](https://apis.io/security/conviva/conviva-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Conviva Scopes](https://apis.io/scopes/conviva/conviva-scopes/)

#### Rate limits (1)

Published request limits.

- [Conviva Rate Limits](https://apis.io/rate-limits/conviva/conviva-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.conviva.ai/)
- [Documentation](https://docs.conviva.ai/)
- [Getting started](https://docs.conviva.ai/api/apis/conviva-vsi-api/metrics-v3-api-guide/)
- [API reference](https://docs.conviva.ai/connect-data/apis/)
- [Sign up](https://www.conviva.ai/get-started)
- [Support](https://www.conviva.ai/contact/)
- [Blog](https://www.conviva.ai/blog/)
- [Compliance](https://www.conviva.ai/security/)
- [Terms of service](https://legal.conviva.ai/terms-of-use/)
- [Privacy policy](https://legal.conviva.ai/privacy-policy/)
- [GitHub](https://github.com/Conviva)
- [Status](https://status.conviva.com/)

## API Evangelist rating

**Kin Score 58.4** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 39.0 |
| Contract governance | 18.2 |
| Operational transparency | 81.6 |
| Developer ergonomics | 71.4 |
| Access clarity | 50.0 |

**Agent readiness 53.6** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/conviva/](https://apis.io/providers/conviva/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Conviva: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/conviva/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
