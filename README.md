# BFE (bfe)
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
