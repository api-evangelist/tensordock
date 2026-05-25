# TensorDock (tensordock)

TensorDock operates a global GPU cloud marketplace that connects independent hardware hosts with customers needing affordable on-demand and spot GPU compute. The platform exposes two REST APIs — the original **Marketplace API (v0)** at `marketplace.tensordock.com` and the newer **Instances API (v2)** at `dashboard.tensordock.com` — to deploy, manage, and scale virtual machines across 100+ locations in 20+ countries with 42+ GPU models ranging from consumer RTX cards to H100 SXM5.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- GPU, Cloud, Marketplace, Compute, Virtual Machines, AI, Machine Learning, Bare Metal, Spot Instances, Containers

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## GPU Inventory and Starting Prices

| Tier | GPU | VRAM | From (USD/hr) |
|---|---|---|---|
| Data Center | NVIDIA H100 SXM5 | 80 GB | $2.25 |
| Data Center | NVIDIA A100 SXM4 | 80 GB | $0.87 |
| Data Center | NVIDIA A100 PCIe | 80 GB | $1.27 |
| Data Center | NVIDIA V100 SXM3 | 32 GB | $0.30 |
| Data Center | NVIDIA V100 SXM2 | 16 GB | $0.21 |
| Professional | NVIDIA RTX 6000 Ada | 48 GB | $0.72 |
| Professional | NVIDIA L40S | 48 GB | $0.49 |
| Professional | NVIDIA L4 | 24 GB | $0.24 |
| Professional | NVIDIA RTX A6000 | 48 GB | $0.42 |
| Consumer | NVIDIA RTX 5090 | 32 GB | $0.56 |
| Consumer | NVIDIA RTX 4090 | 24 GB | $0.32 |
| Consumer | NVIDIA RTX 3090 | 24 GB | $0.17 |
| CPU | Intel Xeon / AMD EPYC | — | $0.012 / vCPU |

Marketplace dynamics mean per-host pricing can vary; the figures above are starting/entry rates. Reserved pricing is available on request from sales, and spot instances are bid-based with soft-validation endpoints.

## APIs

### TensorDock Marketplace API

The original Marketplace REST API (v0) for deploying, managing, starting, stopping, and deleting GPU virtual machines across the global marketplace. Endpoints accept `api_key` + `api_token` authorization pairs as form parameters and cover hostnode discovery, on-demand and spot instance deployment, instance lifecycle, container scaling, and billing balance lookups.

**Human URL:** [https://documenter.getpostman.com/view/20973002/2s8YzMYRDc](https://documenter.getpostman.com/view/20973002/2s8YzMYRDc)

- [OpenAPI](openapi/tensordock-marketplace-api-openapi.yml)
- [Naftiko Capability — Authorization](capabilities/marketplace-auth.yaml)
- [Naftiko Capability — Hostnodes](capabilities/marketplace-hostnodes.yaml)
- [Naftiko Capability — Virtual Machines](capabilities/marketplace-virtual-machines.yaml)
- [Naftiko Capability — Spot](capabilities/marketplace-spot.yaml)
- [Naftiko Capability — Containers](capabilities/marketplace-containers.yaml)
- [Naftiko Capability — Billing](capabilities/marketplace-billing.yaml)

### TensorDock Instances API

The current Instances API (v2) at `https://dashboard.tensordock.com/api/v2/instances` for creating, listing, inspecting, starting, stopping, modifying, and deleting GPU and CPU virtual machines. Uses Bearer-token authentication and a JSON:API-style envelope of `data.type`, `data.id`, and `data.attributes`. Supports both location-based and hostnode-based deployment patterns.

**Human URL:** [https://dashboard.tensordock.com/api/docs/instance-management](https://dashboard.tensordock.com/api/docs/instance-management)

- [OpenAPI](openapi/tensordock-instances-api-openapi.yml)
- [JSON Schema — Instance](json-schema/tensordock-instance-schema.json)
- [JSON-LD](json-ld/tensordock-context.jsonld)
- [Naftiko Capability — Instances](capabilities/instances-instances.yaml)

### TensorDock Secrets API

The Secrets API (v2) for managing SSH keys and generic secrets that are encrypted at rest and in transit and can be attached to instances at deploy time. Two types: `SSHKEY` for SSH authentication and `GENERIC` / `SECRET` for application credentials whose values are not returned after creation.

**Human URL:** [https://dashboard.tensordock.com/api/docs/secrets](https://dashboard.tensordock.com/api/docs/secrets)

- [OpenAPI](openapi/tensordock-secrets-api-openapi.yml)
- [Naftiko Capability — Secrets](capabilities/secrets-secrets.yaml)

## Authentication

- **v0 Marketplace API** — Send `api_key` + `api_token` as form-encoded body parameters (or query string for GET endpoints). Pairs are organization-scoped and can be created without limit at https://dashboard.tensordock.com/api.
- **v2 Instances and Secrets APIs** — Send `Authorization: Bearer <token>` header. Tokens are generated from Developer Settings at https://dashboard.tensordock.com/api.

## Rate Limits

| Surface | Policy |
|---|---|
| Marketplace v0 (`/api/v0/*`) | Best-effort. TensorDock asks customers to "keep API requests reasonable (e.g., 1 request per second)". Bulk-action endpoints can be added on request. |
| Instances API v2 (`/api/v2/*`) | Hard cap of 100 requests per minute per organization. Excess requests are rejected with HTTP 429. |

See [rate-limits/tensordock-rate-limits.yml](rate-limits/tensordock-rate-limits.yml) for the full API Commons Rate Limits 0.1 manifest.

## Plans, FinOps, and Billing

- [Plans / Pricing](plans/tensordock-plans-pricing.yml) — API Commons Plans 0.1
- [Rate Limits](rate-limits/tensordock-rate-limits.yml) — API Commons Rate Limits 0.1
- [FinOps](finops/tensordock-finops.yml) — FOCUS 1.3 / FinOps Foundation framework
- Billing endpoints: `/api/v0/billing/balance`, `/api/v0/billing/revenue`, `/api/v0/billing/summary`

Billing is pro-rated to the microsecond. When the account balance reaches $0, instances are automatically stopped and eventually deleted. Minimum balance of $1 and minimum storage of 100 GB apply to deploys.

## Resources

- [Portal](https://www.tensordock.com)
- [Documentation](https://docs.tensordock.com)
- [API Documentation](https://dashboard.tensordock.com/api/docs)
- [Postman Documentation](https://documenter.getpostman.com/view/20973002/2s8YzMYRDc)
- [Dashboard](https://dashboard.tensordock.com)
- [API Keys](https://dashboard.tensordock.com/api)
- [Blog](https://blog.tensordock.com)
- [Security and Reliability](https://tensordock.com/security)
- [Support](https://marketplace.tensordock.com/support)
- [FAQ](https://marketplace.tensordock.com/faq)
- [Become a Host](https://www.tensordock.com/host.html)
- [User Suggestions](https://tensordock.userjot.com/)

### Legal

- [Terms of Service](https://docs.tensordock.com/legal-information/terms-of-service-tos)
- [Privacy Policy](https://docs.tensordock.com/legal-information/tensordock-privacy-policy)
- [Acceptable Use Policy](https://docs.tensordock.com/legal-information/acceptable-use-policy-aup)
- [Downtime Compensation](https://docs.tensordock.com/legal-information/downtime-compensation)
- [Taxes (VAT, GST)](https://docs.tensordock.com/legal-information/taxes-vat-gst)

### Community

- [Discord](https://discord.gg/Xyzjjuj6zf)
- [Twitter](https://twitter.com/TensorDock)
- [LinkedIn](https://www.linkedin.com/company/tensordock)
- [YouTube](https://www.youtube.com/channel/UCsCAK6krPmRe3Y7Hp5QHXQg)
- [Instagram](https://instagram.com/tensordock)

### Open Source

- [GitHub Organization](https://github.com/tensordock)
- [tensordock-rs (Rust client)](https://github.com/tensordock/tensordock-rs)
- [Unofficial Python SDK](https://pypi.org/project/tensordock/)
- [dashboard-frontend-template (whitelabel storefront)](https://github.com/tensordock/dashboard-frontend-template)
- [wireguard-manager](https://github.com/tensordock/wireguard-manager)
- [tensorblog](https://github.com/tensordock/tensorblog)
- [hosting-install](https://github.com/tensordock/hosting-install)

## Examples

- [List Instances v2](examples/tensordock-list-instances-example.json)
- [Create Instance v2](examples/tensordock-create-instance-example.json)
- [List Hostnodes v0](examples/tensordock-list-hostnodes-example.json)
- [Validate Spot Bid v0](examples/tensordock-spot-validate-new-example.json)
- [Create Secret v2](examples/tensordock-create-secret-example.json)

## Spectral Rules

- [TensorDock Spectral Rules](rules/tensordock-rules.yml)

## Vocabulary

- [TensorDock Vocabulary](vocabulary/tensordock-vocabulary.yml)
