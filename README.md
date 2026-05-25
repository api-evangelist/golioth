# Golioth (golioth)
Golioth is an IoT device management cloud and Firmware SDK for connected hardware. The platform pairs an open-source Firmware SDK (Zephyr RTOS, nRF Connect SDK, ESP-IDF, ModusToolbox, Linux) with a REST Management API at `api.golioth.io`, a web console, and services for OTA firmware updates, device settings, remote procedure calls (RPC), structured time-series data (LightDB Stream), key/value device state (LightDB State), logs, location, and a Pipelines data-routing engine that forwards device data to downstream cloud services. Authentication to the Management API is via project-scoped API keys passed in the `x-api-key` header.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - IoT, Device Management, Firmware, Zephyr, OTA, Embedded, Connectivity

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-25

## APIs

### Golioth Management API
REST API for managing Golioth projects, devices, credentials, blueprints, tags, settings, OTA firmware artifacts and releases, RPC, logs, and Pipelines. Documented with an OpenAPI 3 definition served by the API itself. Authenticated with a project-scoped API key in the `x-api-key` header.

**Human URL:** [https://docs.golioth.io/reference/management-api/](https://docs.golioth.io/reference/management-api/)

- [Documentation](https://docs.golioth.io/reference/management-api/)
- [OpenAPI — local](openapi/golioth-openapi.yml)
- [OpenAPI — upstream](https://api.golioth.io/openapi.json)
- [Swagger](https://api.golioth.io/swagger.json)
- [Authentication](https://docs.golioth.io/reference/management-api/auth)
- [JSON Schema — Device](json-schema/golioth-device-schema.json)
- [JSON Schema — Release](json-schema/golioth-release-schema.json)
- [JSON Schema — Stream Record](json-schema/golioth-stream-record-schema.json)
- [JSON Structure — Device](json-structure/golioth-device-structure.json)
- [JSON Structure — Release](json-structure/golioth-release-structure.json)
- [JSON-LD Context](json-ld/golioth-context.jsonld)
- [Spectral Ruleset](rules/golioth-rules.yml)
- [Naftiko Capability — Projects](capabilities/management-projects.yaml)
- [Naftiko Capability — Devices](capabilities/management-devices.yaml)
- [Naftiko Capability — OTA Firmware](capabilities/management-ota.yaml)
- [Naftiko Capability — LightDB Stream](capabilities/management-stream.yaml)
- [Naftiko Capability — RPC](capabilities/management-rpc.yaml)
- [Naftiko Capability — Device Settings](capabilities/management-settings.yaml)
- [Naftiko Capability — Pipelines](capabilities/management-pipelines.yaml)
- [Naftiko Capability — Logging](capabilities/management-logging.yaml)
- [Naftiko Capability — Tags & Blueprints](capabilities/management-tags-blueprints.yaml)

### Golioth LightDB State
Per-device key/value state store. Devices and cloud services read and write structured state (JSON/CBOR) that is synchronized between device and cloud over CoAP.

**Human URL:** [https://docs.golioth.io/application-services/lightdb/](https://docs.golioth.io/application-services/lightdb/)

- [Documentation](https://docs.golioth.io/application-services/lightdb/)

### Golioth LightDB Stream
Time-series ingest endpoint for streaming sensor and telemetry data from devices. Stored data can be queried and routed downstream via Pipelines.

**Human URL:** [https://docs.golioth.io/application-services/stream/](https://docs.golioth.io/application-services/stream/)

- [Documentation](https://docs.golioth.io/application-services/stream/)
- [JSON Schema — Stream Record](json-schema/golioth-stream-record-schema.json)
- [Naftiko Capability — LightDB Stream](capabilities/management-stream.yaml)
- [Example — Query Stream](examples/golioth-query-stream-example.json)

### Golioth Remote Procedure Call (RPC)
Bidirectional remote-procedure-call service. The cloud invokes device-side methods registered by firmware and receives the response, enabling on-demand diagnostics and control.

**Human URL:** [https://docs.golioth.io/device-management/rpc/](https://docs.golioth.io/device-management/rpc/)

- [Documentation](https://docs.golioth.io/device-management/rpc/)
- [Naftiko Capability — RPC](capabilities/management-rpc.yaml)
- [Example — Invoke RPC](examples/golioth-invoke-rpc-example.json)

### Golioth OTA Firmware Updates
Over-the-air firmware update service. Upload artifacts, group them into releases, target devices by tag or blueprint, and roll out updates with progress tracking and rollback.

**Human URL:** [https://docs.golioth.io/device-management/ota/](https://docs.golioth.io/device-management/ota/)

- [Documentation](https://docs.golioth.io/device-management/ota/)
- [JSON Schema — Release](json-schema/golioth-release-schema.json)
- [JSON Structure — Release](json-structure/golioth-release-structure.json)
- [Naftiko Capability — OTA Firmware](capabilities/management-ota.yaml)
- [Example — Create Release](examples/golioth-create-release-example.json)

### Golioth Device Settings
Cloud-managed settings pushed to one device, a group, or an entire fleet. Firmware subscribes to settings keys and receives updates without requiring a firmware release.

**Human URL:** [https://docs.golioth.io/device-management/settings/](https://docs.golioth.io/device-management/settings/)

- [Documentation](https://docs.golioth.io/device-management/settings/)
- [Naftiko Capability — Device Settings](capabilities/management-settings.yaml)

### Golioth Logging
Centralized device logging. Firmware emits structured log lines that are collected, indexed, and made queryable via the console and API.

**Human URL:** [https://docs.golioth.io/device-management/logging/](https://docs.golioth.io/device-management/logging/)

- [Documentation](https://docs.golioth.io/device-management/logging/)
- [Naftiko Capability — Logging](capabilities/management-logging.yaml)

### Golioth Pipelines
Data routing and transformation engine. Pipelines describe how data arriving from devices is filtered, transformed, and forwarded to downstream destinations such as AWS S3, GCP Pub/Sub, Azure Event Hubs, InfluxDB, MongoDB, and generic webhooks.

**Human URL:** [https://docs.golioth.io/data-routing/](https://docs.golioth.io/data-routing/)

- [Documentation](https://docs.golioth.io/data-routing/)
- [Naftiko Capability — Pipelines](capabilities/management-pipelines.yaml)
- [Example — Create Pipeline](examples/golioth-create-pipeline-example.json)

### Golioth Location
Location service that resolves device position from cellular tower and Wi-Fi access-point observations submitted by firmware, returning latitude/longitude back to the device or downstream system.

**Human URL:** [https://docs.golioth.io/application-services/location/](https://docs.golioth.io/application-services/location/)

- [Documentation](https://docs.golioth.io/application-services/location/)

### Golioth Firmware SDK
Open-source firmware SDK that connects embedded devices to the Golioth cloud over CoAP. Supports Zephyr RTOS, nRF Connect SDK, ESP-IDF, and ModusToolbox.

**Human URL:** [https://github.com/golioth/golioth-firmware-sdk](https://github.com/golioth/golioth-firmware-sdk)

- [Repository](https://github.com/golioth/golioth-firmware-sdk)

### Golioth Python Tools
Python tooling that wraps the Management API for scripting, automation, and CLI-driven workflows against Golioth projects.

**Human URL:** [https://github.com/golioth/python-golioth-tools](https://github.com/golioth/python-golioth-tools)

- [Repository](https://github.com/golioth/python-golioth-tools)

### Golioth tinymcp
Open-source implementation of the Model Context Protocol (MCP) for resource-constrained embedded devices, enabling large language models — including Anthropic's Claude — to observe and control firmware via MCP tools.

**Human URL:** [https://github.com/golioth/tinymcp](https://github.com/golioth/tinymcp)

- [Repository](https://github.com/golioth/tinymcp)

### Golioth Pouch
Non-IP device-to-cloud transport protocol from Golioth, with a companion Bluetooth gateway reference implementation (`pouch-gateway`) for relaying pouch traffic to the Golioth cloud.

**Human URL:** [https://github.com/golioth/pouch](https://github.com/golioth/pouch)

- [Repository](https://github.com/golioth/pouch)

## Common Properties

- [Website](https://golioth.io/)
- [Documentation](https://docs.golioth.io/)
- [GitHub Organization](https://github.com/golioth)
- [Console](https://console.golioth.io/)
- [Forum](https://forum.golioth.io/)
- [Blog](https://blog.golioth.io/)
- [Training](https://training.golioth.io/)
- [Reference Designs](https://projects.golioth.io/)
- [Pricing](https://golioth.io/pricing)
- [LinkedIn](https://www.linkedin.com/company/golioth/)
- [LLMs.txt](https://docs.golioth.io/llms.txt)

## Integrations

Zephyr RTOS, nRF Connect SDK, ESP-IDF, ModusToolbox, AWS, Google Cloud, Microsoft Azure, InfluxDB, MongoDB, Anthropic.

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Golioth Management API](openapi/golioth-openapi.yml)

### JSON Schema

- [Device](json-schema/golioth-device-schema.json)
- [Release](json-schema/golioth-release-schema.json)
- [Stream Record](json-schema/golioth-stream-record-schema.json)

### JSON Structure

- [Device](json-structure/golioth-device-structure.json)
- [Release](json-structure/golioth-release-structure.json)

### JSON-LD

- [Golioth Context](json-ld/golioth-context.jsonld)

### Capabilities (Naftiko)

- [Projects](capabilities/management-projects.yaml)
- [Devices](capabilities/management-devices.yaml)
- [OTA Firmware](capabilities/management-ota.yaml)
- [LightDB Stream](capabilities/management-stream.yaml)
- [RPC](capabilities/management-rpc.yaml)
- [Device Settings](capabilities/management-settings.yaml)
- [Pipelines](capabilities/management-pipelines.yaml)
- [Logging](capabilities/management-logging.yaml)
- [Tags & Blueprints](capabilities/management-tags-blueprints.yaml)

### Examples

- [Create Device](examples/golioth-create-device-example.json)
- [Create Release](examples/golioth-create-release-example.json)
- [Invoke RPC](examples/golioth-invoke-rpc-example.json)
- [Query LightDB Stream](examples/golioth-query-stream-example.json)
- [Create Pipeline](examples/golioth-create-pipeline-example.json)

### Spectral Rules

- [Golioth Rules](rules/golioth-rules.yml)

### Vocabulary

- [Golioth Vocabulary](vocabulary/golioth-vocabulary.yml)

### Commercial Artifacts

- [Plans / Pricing](plans/golioth-plans-pricing.yml)
- [Rate Limits](rate-limits/golioth-rate-limits.yml)
- [FinOps Definition](finops/golioth-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
