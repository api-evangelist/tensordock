# TensorDock

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

TensorDock operates a global GPU cloud marketplace that connects independent hardware hosts with customers needing affordable on-demand and spot GPU compute. The platform exposes two REST APIs — the original Marketplace API (v0) at marketplace.tensordock.com and the newer Instances API (v2) at dashboard.tensordock.com — to deploy, manage, and scale virtual machines across 100+ locations in 20+ countries with 42+ GPU models ranging from consumer RTX cards to H100 SXM5. TensorDock targets AI startups, researchers, rendering shops, and gaming services that need cost-effective compute (advertised at up to 80% less than hyperscalers) without quotas or long-term commitments.

**Areas:** GPU · Cloud · Marketplace · Compute · Virtual Machines · Artificial Intelligence · Machine Learning · Bare Metal · Spot Instances · Containers

## TensorDock on APIs.io

Everything profiled for TensorDock is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/tensordock/](https://apis.io/providers/tensordock/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [TensorDock Instances API](https://apis.io/apis/tensordock/tensordock-instances-api/) — The current TensorDock Instances API (v2) at https://dashboard.tensordock.com/api/v2/instances for creating, listing, inspecting, starting, stopping,…
- [TensorDock Secrets API](https://apis.io/apis/tensordock/tensordock-secrets-api/) — The TensorDock Secrets API (v2) for managing SSH keys and generic secrets that are encrypted at rest and in transit and can be attached to instances at…
- [TensorDock Authorization API](https://apis.io/apis/tensordock/tensordock-authorization-api/) — Verify and list API authorization pairs
- [TensorDock Billing API](https://apis.io/apis/tensordock/tensordock-billing-api/) — Retrieve balance, revenue, and monthly summaries
- [TensorDock Containers API](https://apis.io/apis/tensordock/tensordock-containers-api/) — Deploy, scale, terminate, and inspect containers
- [TensorDock Hostnodes API](https://apis.io/apis/tensordock/tensordock-hostnodes-api/) — Discover available hostnodes and GPU/CPU configurations
- [TensorDock Instant VMs API](https://apis.io/apis/tensordock/tensordock-instant-vms-api/) — Deploy and inspect pre-configured Instant VMs
- [TensorDock Spot API](https://apis.io/apis/tensordock/tensordock-spot-api/) — Validate spot instance pricing for new and existing instances
- [TensorDock Virtual Machines API](https://apis.io/apis/tensordock/tensordock-virtual-machines-api/) — Deploy, list, start, stop, modify, and delete virtual machines

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Tensordock Agentic Access](https://apis.io/agentic-access/tensordock/tensordock-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [TensorDock Hostnode](https://apis.io/schemas/tensordock/tensordock-hostnode/)
- [TensorDock Instance](https://apis.io/schemas/tensordock/tensordock-instance/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Tensordock Context](https://apis.io/jsonld/tensordock/tensordock-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Tensordock Vocabulary](https://apis.io/vocabularies/tensordock/tensordock-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Tensordock Create Instance Example](https://apis.io/examples/tensordock/tensordock-create-instance-example/)
- [Tensordock Create Secret Example](https://apis.io/examples/tensordock/tensordock-create-secret-example/)
- [Tensordock List Hostnodes Example](https://apis.io/examples/tensordock/tensordock-list-hostnodes-example/)
- [Tensordock List Instances Example](https://apis.io/examples/tensordock/tensordock-list-instances-example/)
- [Tensordock Spot Validate New Example](https://apis.io/examples/tensordock/tensordock-spot-validate-new-example/)

#### Collections (11)

Postman and Open Collection request collections.

- [TensorDock Marketplace Authorization API](https://apis.io/collections/tensordock/open-tensordock-authorization-api/)
- [TensorDock Marketplace Billing API](https://apis.io/collections/tensordock/open-tensordock-billing-api/)
- [TensorDock Marketplace Containers API](https://apis.io/collections/tensordock/open-tensordock-containers-api/)
- [TensorDock Marketplace Hostnodes API](https://apis.io/collections/tensordock/open-tensordock-hostnodes-api/)
- [TensorDock Instances API](https://apis.io/collections/tensordock/open-tensordock-instances-api/)
- [TensorDock Marketplace Instant VMs API](https://apis.io/collections/tensordock/open-tensordock-instant-vms-api/)
- [TensorDock Instances Secrets API](https://apis.io/collections/tensordock/open-tensordock-secrets-api/)
- [TensorDock Marketplace Spot API](https://apis.io/collections/tensordock/open-tensordock-spot-api/)
- [TensorDock Marketplace Virtual Machines API](https://apis.io/collections/tensordock/open-tensordock-virtual-machines-api/)
- [TensorDock Instances API](https://apis.io/collections/tensordock/postman-tensordock-instances-api/)
- [TensorDock Instances Secrets API](https://apis.io/collections/tensordock/postman-tensordock-secrets-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [TensorDock — jsonschema rules](https://apis.io/rules/tensordock/tensordock-jsonschema-spectral-rules/)
- [TensorDock API Rules](https://apis.io/rules/tensordock/tensordock-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Tensordock Authentication](https://apis.io/security/tensordock/tensordock-authentication/)
- [Tensordock Domain Security](https://apis.io/security/tensordock/tensordock-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Tensordock Plans Pricing](https://apis.io/plans/tensordock/tensordock-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Tensordock Rate Limits](https://apis.io/rate-limits/tensordock/tensordock-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Tensordock Finops](https://apis.io/finops/tensordock/tensordock-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.tensordock.com/)
- [Documentation](https://docs.tensordock.com)
- [Getting started](https://dashboard.tensordock.com/api/docs/getting-started)
- [Pricing](https://marketplace.tensordock.com)
- [Support](https://marketplace.tensordock.com/support)
- [Blog](https://blog.tensordock.com)
- [Trust centre](https://tensordock.com/security)
- [Terms of service](https://docs.tensordock.com/legal-information/terms-of-service-tos)
- [Privacy policy](https://docs.tensordock.com/legal-information/tensordock-privacy-policy)
- [GitHub](https://github.com/tensordock)

## API Evangelist rating

**Kin Score 54.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 55.0 |
| Contract governance | 13.6 |
| Operational transparency | 7.9 |
| Developer ergonomics | 65.5 |
| Access clarity | 92.1 |

**Agent readiness 19.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/tensordock/](https://apis.io/providers/tensordock/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for TensorDock: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/tensordock/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
