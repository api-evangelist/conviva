# Conviva

Conviva is the streaming-media and digital-experience analytics company behind Experience-Centric
Operations (ECO) — a real-time, full-census operational data platform that stitches client-side
telemetry from its Sensor SDKs into stateful, per-viewer experience analytics for video streamers,
broadcasters and app publishers.

- Website: https://www.conviva.ai/
- Docs: https://docs.conviva.ai/
- APIs: https://docs.conviva.ai/connect-data/apis/
- GitHub: https://github.com/Conviva
- Status: https://status.conviva.com/

## API surface

| API | Base URL | Auth |
|---|---|---|
| Metrics V3 | `https://api.conviva.com/insights/3.0/metrics` | HTTP Basic (API key pair) |
| Real-Time Metrics V3 | `https://api.conviva.com/insights/3.0/real-time-metrics` | HTTP Basic |
| Sessions V3 | `https://api.conviva.com/insights/3.0/sessions` | HTTP Basic |
| AI Alerts | `https://api.conviva.com/insights/2.6/ai-alerts` | HTTP Basic |
| Bulk Filters | `https://api.conviva.com/bulk_filters` | HTTP Basic |
| Precision Policy | `https://api.conviva.com/precision/v1.0/policies` | HTTP Basic + Precision Admin |
| PII Opt-Out | `https://api.conviva.com/pii-opt-out` | HTTP Basic |
| Validation Timeline v2 | `https://api.conviva.com/validation/v2/timeline` | HTTP Basic |
| MCP Server | `https://mcp.conviva.com/mcp` | OAuth 2.1 / HTTP Basic |
| DPI MCP Server | `https://dpi-mcp.conviva.com/mcp` | OAuth 2.1 (Okta) |

## Notable

- **Two hosted MCP servers**, both OAuth 2.1 protected resources with RFC 8414 + RFC 9728 discovery,
  RFC 7591 dynamic client registration and PKCE S256. `tools/list` is auth-gated on both.
- **Provider-published Agent Skills.** Conviva ships three of its own Agent Skills through a Claude
  plugin marketplace at `github.com/Conviva/mcp-marketplace`; they are mirrored verbatim in
  `skills/`. This is a genuinely rare artifact — most providers publish none.
- **No OpenAPI.** Conviva's own APIs page states the Scalar reference "renders a placeholder until
  specs exist." Every standard spec path was probed on every host and missed.
- **The agent surface is read-only by construction.** Every write Conviva exposes over REST
  (filters, Precision policy, PII opt-out) is absent from its MCP servers.
- **ISO/IEC 27001:2022 certified.** SOC 1/SOC 2 are inherited from hosting providers, not Conviva's
  own audits.

## Artifacts

`apis.yml` · `asyncapi/` (webhooks) · `authentication/` · `changelog/` · `conformance/` ·
`conventions/` · `errors/` · `lifecycle/` · `llms/` · `mcp/` (server + tool crosswalk) ·
`packages/` · `rate-limits/` · `scopes/` · `security/` · `skills/` · `well-known/`
