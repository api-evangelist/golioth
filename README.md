# Golioth

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

Golioth is an IoT device management cloud and firmware SDK for connected hardware. The platform pairs an open-source Firmware SDK (Zephyr RTOS, nRF Connect SDK, ESP-IDF, ModusToolbox, Linux) with a REST Management API at api.golioth.io, a web console, and services for OTA firmware updates, device settings, remote procedure calls (RPC), structured time-series data (LightDB Stream), key/value device state (LightDB State), logs, location, and a Pipelines data-routing engine that forwards device data to downstream cloud services. Authentication to the Management API is via project-scoped API keys passed in the x-api-key header.

**Areas:** IoT · Device Management · Firmware · Zephyr · OTA · Embedded · Connectivity

## Golioth on APIs.io

Everything profiled for Golioth is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/golioth/](https://apis.io/providers/golioth/)** — or go straight to one of the APIs or properties below.

### APIs (45)

- [Golioth LightDB State](https://apis.io/apis/golioth/lightdb-state/) — Per-device key/value state store. Devices and cloud services read and write structured state (JSON/CBOR) that is synchronized between device and cloud over…
- [Golioth LightDB Stream](https://apis.io/apis/golioth/lightdb-stream/) — Time-series ingest endpoint for streaming sensor and telemetry data from devices. Stored data can be queried and routed downstream via Pipelines.
- [Golioth Remote Procedure Call (RPC)](https://apis.io/apis/golioth/rpc/) — Bidirectional remote-procedure-call service. The cloud invokes device-side methods registered by firmware and receives the response, enabling on-demand…
- [Golioth OTA Firmware Updates](https://apis.io/apis/golioth/ota/) — Over-the-air firmware update service. Upload artifacts, group them into releases, target devices by tag or blueprint, and roll out updates with progress…
- [Golioth Device Settings](https://apis.io/apis/golioth/settings/) — Cloud-managed settings pushed to one device, a group, or an entire fleet. Firmware subscribes to settings keys and receives updates without requiring a…
- [Golioth Logging](https://apis.io/apis/golioth/logging/) — Centralized device logging. Firmware emits structured log lines that are collected, indexed, and made queryable via the console and API.
- [Golioth Pipelines](https://apis.io/apis/golioth/pipelines/) — Data routing and transformation engine. Pipelines describe how data arriving from devices is filtered, transformed, and forwarded to downstream destinations…
- [Golioth Location](https://apis.io/apis/golioth/location/) — Location service that resolves device position from cellular tower and Wi-Fi access-point observations submitted by firmware, returning latitude/longitude…
- [Golioth Firmware SDK](https://apis.io/apis/golioth/firmware-sdk/) — Open-source firmware SDK that connects embedded devices to the Golioth cloud over CoAP. Supports Zephyr RTOS, nRF Connect SDK, ESP-IDF, and ModusToolbox.…
- [Golioth Python Tools](https://apis.io/apis/golioth/python-tools/) — Python tooling that wraps the Management API for scripting, automation, and CLI-driven workflows against Golioth projects.
- [Golioth Tinymcp API](https://apis.io/apis/golioth/tinymcp/) — Open-source implementation of the Model Context Protocol (MCP) for resource-constrained embedded devices, enabling large language models to observe and…
- [Golioth Pouch](https://apis.io/apis/golioth/pouch/) — Non-IP device-to-cloud transport protocol from Golioth, with a companion Bluetooth gateway reference implementation (pouch-gateway) for relaying pouch…
- [Golioth Access API](https://apis.io/apis/golioth/golioth-access-api/) — The Access API from Golioth — 6 operation(s) for access.
- [Golioth API Keys API](https://apis.io/apis/golioth/golioth-api-keys-api/) — The API Keys API from Golioth — 2 operation(s) for api keys.
- [Golioth Artifacts API](https://apis.io/apis/golioth/golioth-artifacts-api/) — The Artifacts API from Golioth — 3 operation(s) for artifacts.
- [Golioth Billing API](https://apis.io/apis/golioth/golioth-billing-api/) — The Billing API from Golioth — 1 operation(s) for billing.
- [Golioth Blueprints API](https://apis.io/apis/golioth/golioth-blueprints-api/) — The Blueprints API from Golioth — 2 operation(s) for blueprints.
- [Golioth Boards API](https://apis.io/apis/golioth/golioth-boards-api/) — The Boards API from Golioth — 2 operation(s) for boards.
- [Golioth Certificates API](https://apis.io/apis/golioth/golioth-certificates-api/) — The Certificates API from Golioth — 2 operation(s) for certificates.
- [Golioth Cohorts API](https://apis.io/apis/golioth/golioth-cohorts-api/) — The Cohorts API from Golioth — 2 operation(s) for cohorts.
- [Golioth Credentials API](https://apis.io/apis/golioth/golioth-credentials-api/) — The Credentials API from Golioth — 4 operation(s) for credentials.
- [Golioth Deployments API](https://apis.io/apis/golioth/golioth-deployments-api/) — The Deployments API from Golioth — 2 operation(s) for deployments.
- [Golioth Devices API](https://apis.io/apis/golioth/golioth-devices-api/) — The Devices API from Golioth — 2 operation(s) for devices.
- [Golioth Firmware API](https://apis.io/apis/golioth/golioth-firmware-api/) — The Firmware API from Golioth — 1 operation(s) for firmware.
- [Golioth Integrations API](https://apis.io/apis/golioth/golioth-integrations-api/) — The Integrations API from Golioth — 5 operation(s) for integrations.
- [Golioth LightDB API](https://apis.io/apis/golioth/golioth-lightdb-api/) — The LightDB API from Golioth — 2 operation(s) for lightdb.
- [Golioth LightDB Stream API](https://apis.io/apis/golioth/golioth-lightdb-stream-api/) — The LightDB Stream API from Golioth — 2 operation(s) for lightdb stream.
- [Golioth Location API](https://apis.io/apis/golioth/golioth-location-api/) — The Location API from Golioth — 1 operation(s) for location.
- [Golioth Logs API](https://apis.io/apis/golioth/golioth-logs-api/) — The Logs API from Golioth — 2 operation(s) for logs.
- [Golioth Networks API](https://apis.io/apis/golioth/golioth-networks-api/) — The Networks API from Golioth — 4 operation(s) for networks.
- [Golioth Notifications API](https://apis.io/apis/golioth/golioth-notifications-api/) — The Notifications API from Golioth — 1 operation(s) for notifications.
- [Golioth Organizations API](https://apis.io/apis/golioth/golioth-organizations-api/) — The Organizations API from Golioth — 2 operation(s) for organizations.
- [Golioth OTAEvents API](https://apis.io/apis/golioth/golioth-otaevents-api/) — The OTAEvents API from Golioth — 2 operation(s) for otaevents.
- [Golioth Packages API](https://apis.io/apis/golioth/golioth-packages-api/) — The Packages API from Golioth — 2 operation(s) for packages.
- [Golioth Pipelines API](https://apis.io/apis/golioth/golioth-pipelines-api/) — The Pipelines API from Golioth — 5 operation(s) for pipelines.
- [Golioth PKI API](https://apis.io/apis/golioth/golioth-pki-api/) — The PKI API from Golioth — 5 operation(s) for pki.
- [Golioth Project Config API](https://apis.io/apis/golioth/golioth-project-config-api/) — The Project Config API from Golioth — 2 operation(s) for project config.
- [Golioth Projects API](https://apis.io/apis/golioth/golioth-projects-api/) — The Projects API from Golioth — 2 operation(s) for projects.
- [Golioth Provisioning API](https://apis.io/apis/golioth/golioth-provisioning-api/) — The Provisioning API from Golioth — 2 operation(s) for provisioning.
- [Golioth Releases API](https://apis.io/apis/golioth/golioth-releases-api/) — The Releases API from Golioth — 2 operation(s) for releases.
- [Golioth Remote Procedure Call API](https://apis.io/apis/golioth/golioth-remote-procedure-call-api/) — The Remote Procedure Call API from Golioth — 1 operation(s) for remote procedure call.
- [Golioth Secrets API](https://apis.io/apis/golioth/golioth-secrets-api/) — The Secrets API from Golioth — 2 operation(s) for secrets.
- [Golioth Settings API](https://apis.io/apis/golioth/golioth-settings-api/) — The Settings API from Golioth — 4 operation(s) for settings.
- [Golioth Tags API](https://apis.io/apis/golioth/golioth-tags-api/) — The Tags API from Golioth — 2 operation(s) for tags.
- [Golioth Usage API](https://apis.io/apis/golioth/golioth-usage-api/) — The Usage API from Golioth — 5 operation(s) for usage.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Golioth Agentic Access](https://apis.io/agentic-access/golioth/golioth-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Golioth Device](https://apis.io/schemas/golioth/golioth-device/)
- [Golioth Release](https://apis.io/schemas/golioth/golioth-release/)
- [Golioth Stream Record](https://apis.io/schemas/golioth/golioth-stream-record/)

#### JSON Structure (2)

Data models expressed in JSON Structure.

- [Golioth Device Structure](https://apis.io/json-structure/golioth/golioth-device-structure/)
- [Golioth Release Structure](https://apis.io/json-structure/golioth/golioth-release-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Golioth Context](https://apis.io/jsonld/golioth/golioth-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Golioth Vocabulary](https://apis.io/vocabularies/golioth/golioth-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Golioth Create Device Example](https://apis.io/examples/golioth/golioth-create-device-example/)
- [Golioth Create Pipeline Example](https://apis.io/examples/golioth/golioth-create-pipeline-example/)
- [Golioth Create Release Example](https://apis.io/examples/golioth/golioth-create-release-example/)
- [Golioth Invoke Rpc Example](https://apis.io/examples/golioth/golioth-invoke-rpc-example/)
- [Golioth Query Stream Example](https://apis.io/examples/golioth/golioth-query-stream-example/)

#### Collections (34)

Postman and Open Collection request collections.

- [Golioth Management API](https://apis.io/collections/golioth/open-golioth/)
- [Golioth Management Access API](https://apis.io/collections/golioth/open-golioth-access-api/)
- [Golioth Management Access API Keys API](https://apis.io/collections/golioth/open-golioth-api-keys-api/)
- [Golioth Management Access Artifacts API](https://apis.io/collections/golioth/open-golioth-artifacts-api/)
- [Golioth Management Access Billing API](https://apis.io/collections/golioth/open-golioth-billing-api/)
- [Golioth Management Access Blueprints API](https://apis.io/collections/golioth/open-golioth-blueprints-api/)
- [Golioth Management Access Boards API](https://apis.io/collections/golioth/open-golioth-boards-api/)
- [Golioth Management Access Certificates API](https://apis.io/collections/golioth/open-golioth-certificates-api/)
- [Golioth Management Access Cohorts API](https://apis.io/collections/golioth/open-golioth-cohorts-api/)
- [Golioth Management Access Credentials API](https://apis.io/collections/golioth/open-golioth-credentials-api/)
- [Golioth Management Access Deployments API](https://apis.io/collections/golioth/open-golioth-deployments-api/)
- [Golioth Management Access Devices API](https://apis.io/collections/golioth/open-golioth-devices-api/)
- [Golioth Management Access Firmware API](https://apis.io/collections/golioth/open-golioth-firmware-api/)
- [Golioth Management Access Integrations API](https://apis.io/collections/golioth/open-golioth-integrations-api/)
- [Golioth Management Access LightDB API](https://apis.io/collections/golioth/open-golioth-lightdb-api/)
- [Golioth Management Access LightDB Stream API](https://apis.io/collections/golioth/open-golioth-lightdb-stream-api/)
- [Golioth Management Access Location API](https://apis.io/collections/golioth/open-golioth-location-api/)
- [Golioth Management Access Logs API](https://apis.io/collections/golioth/open-golioth-logs-api/)
- [Golioth Management Access Networks API](https://apis.io/collections/golioth/open-golioth-networks-api/)
- [Golioth Management Access Notifications API](https://apis.io/collections/golioth/open-golioth-notifications-api/)
- [Golioth Management Access Organizations API](https://apis.io/collections/golioth/open-golioth-organizations-api/)
- [Golioth Management Access OTAEvents API](https://apis.io/collections/golioth/open-golioth-otaevents-api/)
- [Golioth Management Access Packages API](https://apis.io/collections/golioth/open-golioth-packages-api/)
- [Golioth Management Access Pipelines API](https://apis.io/collections/golioth/open-golioth-pipelines-api/)
- [Golioth Management Access PKI API](https://apis.io/collections/golioth/open-golioth-pki-api/)
- …and 9 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Golioth — jsonschema rules](https://apis.io/rules/golioth/golioth-jsonschema-spectral-rules/)
- [Golioth API Rules](https://apis.io/rules/golioth/golioth-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Golioth Authentication](https://apis.io/security/golioth/golioth-authentication/)
- [Golioth Domain Security](https://apis.io/security/golioth/golioth-domain-security/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Golioth Plans Pricing](https://apis.io/plans/golioth/golioth-plans-pricing/)
- [Golioth Price Estimates](https://apis.io/plans/golioth/golioth-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Golioth Rate Limits](https://apis.io/rate-limits/golioth/golioth-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Golioth Finops](https://apis.io/finops/golioth/golioth-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://golioth.io/)
- [Documentation](https://docs.golioth.io/)
- [Pricing](https://golioth.io/pricing)
- [Blog](https://blog.golioth.io/)

## API Evangelist rating

**Kin Score 45.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 62.9 |
| Contract governance | 27.3 |
| Operational transparency | 26.3 |
| Developer ergonomics | 28.6 |
| Access clarity | 42.1 |

**Agent readiness 21.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
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
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/golioth/](https://apis.io/providers/golioth/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Golioth: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/golioth/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
