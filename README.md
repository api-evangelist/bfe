# BFE (bfe)

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

BFE (Beyond Front End) is an open-source layer 7 load balancer developed by Baidu, providing advanced traffic routing, forwarding, and load balancing capabilities with support for HTTP, HTTPS, HTTP/2, WebSocket, TLS, and gRPC. BFE is a CNCF sandbox project licensed under Apache 2.0.

**URL:** [https://www.bfe-networks.net/en_us/](https://www.bfe-networks.net/en_us/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Load Balancer, Networking, Open Source, Traffic Management, CNCF, Baidu

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-21

## APIs

### BFE Management API
The BFE Management API provides internal monitoring metrics, configuration reload, and Go pprof profiling endpoints. This API should only be exposed on internal networks.

**Human URL:** [https://www.bfe-networks.net/en_us/operation/api/](https://www.bfe-networks.net/en_us/operation/api/)

#### Tags:

 - Management, Monitoring, Configuration, Observability

#### Properties

- [Documentation](https://www.bfe-networks.net/en_us/operation/api/)
- [OpenAPI](openapi/bfe-management-api.yaml)

## Common Properties

- [Portal](https://www.bfe-networks.net/en_us/)
- [Documentation](https://www.bfe-networks.net/en_us/)
- [GitHubOrganization](https://github.com/bfenetworks)
- [GitHubRepository](https://github.com/bfenetworks/bfe)
- [SpectralRules](rules/bfe-spectral-rules.yml)
- [NaftikoCapability](capabilities/load-balancer-management.yaml)
- [Vocabulary](vocabulary/bfe-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Layer 7 Load Balancing | Advanced HTTP/HTTPS/HTTP2 load balancing with pluggable algorithms. |
| Plugin Framework | Extensible plugin system enabling custom traffic management logic. |
| Multi-tenancy | Isolated configuration and routing per tenant. |
| Advanced Routing | DSL-based routing rules for fine-grained traffic control. |
| Protocol Support | HTTP, HTTPS, SPDY, HTTP/2, gRPC, WebSocket, TLS, FastCGI protocols. |
| Observability | Built-in metrics, logging, and distributed tracing integration. |
| Dynamic Configuration | Hot reload of routing and load balancing configuration without restart. |
| CNCF Sandbox | Hosted as a CNCF sandbox project with active community governance. |

## Use Cases

| Name | Description |
|------|-------------|
| Enterprise API Gateway | Route and load balance API traffic with per-tenant isolation. |
| Microservices Traffic Management | Manage east-west and north-south traffic in microservices architectures. |
| TLS Termination | Terminate TLS/HTTPS at the edge and forward to backend HTTP services. |
| A/B Testing | Route fractions of traffic to canary deployments using routing rules. |
| DDoS Mitigation | Use traffic management plugins to detect and mitigate DDoS attacks. |

## Integrations

| Name | Description |
|------|-------------|
| Prometheus | Export metrics to Prometheus for monitoring and alerting. |
| Kubernetes | Deploy BFE as an ingress controller in Kubernetes clusters. |
| Docker | Run BFE in Docker containers for containerized deployments. |
| Grafana | Visualize BFE metrics in Grafana dashboards. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [BFE Management API](openapi/bfe-management-api.yaml)

### JSON Schema

- [bfe-monitor-categories-response-schema.json](json-schema/bfe-monitor-categories-response-schema.json)
- [bfe-monitor-metrics-response-schema.json](json-schema/bfe-monitor-metrics-response-schema.json)
- [bfe-reload-entries-response-schema.json](json-schema/bfe-reload-entries-response-schema.json)
- [bfe-reload-entry-schema.json](json-schema/bfe-reload-entry-schema.json)
- [bfe-reload-response-schema.json](json-schema/bfe-reload-response-schema.json)

### JSON-LD

- [bfe-context.jsonld](json-ld/bfe-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [BFE Management API](capabilities/shared/management-api.yaml) — 3 operations for load balancer management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Load Balancer Management](capabilities/load-balancer-management.yaml) | BFE Management | 3 | Platform Engineer, SRE |

## Vocabulary

- [BFE Vocabulary](vocabulary/bfe-vocabulary.yaml)

## Rules

- [BFE Spectral Rules](rules/bfe-spectral-rules.yml) — 21 rules across 8 categories enforcing BFE API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
