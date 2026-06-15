# TensorDock (tensordock)

TensorDock operates a global GPU cloud marketplace that connects independent hardware hosts with customers needing affordable on-demand and spot GPU compute. The platform exposes two REST APIs — the original Marketplace API (v0) at marketplace.tensordock.com and the newer Instances API (v2) at dashboard.tensordock.com — to deploy, manage, and scale virtual machines across 100+ locations in 20+ countries with 42+ GPU models ranging from consumer RTX cards to H100 SXM5. TensorDock targets AI startups, researchers, rendering shops, and gaming services that need cost-effective compute (advertised at up to 80% less than hyperscalers) without quotas or long-term commitments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- GPU
- Cloud
- Marketplace
- Compute
- Virtual Machines
- AI
- Machine Learning
- Bare Metal
- Spot Instances
- Containers

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### TensorDock Marketplace API

The original TensorDock Marketplace REST API (v0) for deploying, managing, starting, stopping, and deleting GPU virtual machines across the global marketplace of independent hardware hosts. Endpoints accept api_key + api_token authorization pairs as form parameters and cover hostnode discovery, on-demand and spot instance deployment, instance lifecycle, container scaling, and billing balance lookups.

- **Human URL:** [https://documenter.getpostman.com/view/20973002/2s8YzMYRDc](https://documenter.getpostman.com/view/20973002/2s8YzMYRDc)

#### Tags

- GPU
- Cloud
- Compute
- Marketplace
- Virtual Machines

#### Properties

- [Documentation](https://documenter.getpostman.com/view/20973002/2s8YzMYRDc)
- [OpenAPI](openapi/tensordock-marketplace-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### TensorDock Instances API

The current TensorDock Instances API (v2) at https://dashboard.tensordock.com/api/v2/instances for creating, listing, inspecting, starting, stopping, modifying, and deleting GPU and CPU virtual machines. Uses Bearer token authentication and a JSON:API-style envelope of `data.type`, `data.id`, and `data.attributes`. Supports both location-based and hostnode-based deployment patterns.

- **Human URL:** [https://dashboard.tensordock.com/api/docs/instance-management](https://dashboard.tensordock.com/api/docs/instance-management)

#### Tags

- GPU
- Cloud
- Compute
- Instances
- Virtual Machines

#### Properties

- [Documentation](https://dashboard.tensordock.com/api/docs/instance-management)
- [Documentation](https://dashboard.tensordock.com/api/docs/instance-creation)
- [OpenAPI](openapi/tensordock-instances-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tensordock-instances-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tensordock-instances-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tensordock-instance-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/tensordock-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### TensorDock Secrets API

The TensorDock Secrets API (v2) for managing SSH keys and generic secrets that are encrypted at rest and in transit and can be attached to instances at deploy time. Two secret types are supported — `SSHKEY` for SSH authentication and `SECRET`/`GENERIC` for application credentials whose values are not returned after creation.

- **Human URL:** [https://dashboard.tensordock.com/api/docs/secrets](https://dashboard.tensordock.com/api/docs/secrets)

#### Tags

- GPU
- Cloud
- Secrets
- SSH Keys
- Credentials

#### Properties

- [Documentation](https://dashboard.tensordock.com/api/docs/secrets)
- [OpenAPI](openapi/tensordock-secrets-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tensordock-secrets-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tensordock-secrets-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.tensordock.com)
- [Documentation](https://docs.tensordock.com)
- [Documentation](https://dashboard.tensordock.com/api/docs)
- [Documentation](https://documenter.getpostman.com/view/20973002/2s8YzMYRDc)
- [Getting Started](https://dashboard.tensordock.com/api/docs/getting-started)
- [Console](https://dashboard.tensordock.com)
- [Sandbox](https://dashboard.tensordock.com/deploy)
- [Sandbox](https://dashboard.tensordock.com/deploy_cpu)
- [Sign Up](https://dashboard.tensordock.com/api)
- [Blog](https://blog.tensordock.com)
- [Trust Center](https://tensordock.com/security)
- [Documentation](https://docs.tensordock.com/legal-information/legal-information)
- [Terms of Service](https://docs.tensordock.com/legal-information/terms-of-service-tos)
- [Privacy Policy](https://docs.tensordock.com/legal-information/tensordock-privacy-policy)
- [Terms of Service](https://docs.tensordock.com/legal-information/acceptable-use-policy-aup)
- [Documentation](https://docs.tensordock.com/legal-information/downtime-compensation)
- [Documentation](https://docs.tensordock.com/legal-information/taxes-vat-gst)
- [Support](https://marketplace.tensordock.com/support)
- [Support](https://marketplace.tensordock.com/faq)
- [Forum](https://tensordock.userjot.com/)
- [Twitter](https://twitter.com/TensorDock)
- [LinkedIn](https://www.linkedin.com/company/tensordock)
- [Instagram](https://instagram.com/tensordock)
- [YouTube](https://www.youtube.com/channel/UCsCAK6krPmRe3Y7Hp5QHXQg)
- [Forum](https://discord.gg/Xyzjjuj6zf)
- [GitHub Organization](https://github.com/tensordock)
- [SDK](https://github.com/tensordock/tensordock-rs)
- [SDK](https://pypi.org/project/tensordock/)
- [Tool](https://github.com/tensordock/dashboard-frontend-template)
- [Tool](https://github.com/tensordock/wireguard-manager)
- [Tool](https://github.com/tensordock/tensorblog)
- [Tool](https://github.com/tensordock/hosting-install)
- [Documentation](https://docs.tensordock.com/virtual-machines/introduction-to-core-compute-vms)
- [Documentation](https://docs.tensordock.com/virtual-machines/spot-instances)
- [Documentation](https://docs.tensordock.com/virtual-machines/cloud-init)
- [Documentation](https://docs.tensordock.com/virtual-machines/how-to-ssh-into-your-instance)
- [Documentation](https://docs.tensordock.com/virtual-machines/how-to-rdp-into-your-instance)
- [Documentation](https://docs.tensordock.com/whitelabel/overview)
- [Documentation](https://docs.tensordock.com/whitelabel/setting-up-a-storefront)
- [Sign Up](https://www.tensordock.com/host.html)
- [Plans](plans/tensordock-plans-pricing.yml)
- [Rate Limits](rate-limits/tensordock-rate-limits.yml)
- [Fin Ops](finops/tensordock-finops.yml)
- [Pricing](https://marketplace.tensordock.com)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
