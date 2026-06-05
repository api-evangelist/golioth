# Golioth (golioth)

Golioth is an IoT device management cloud and firmware SDK for connected hardware. The platform pairs an open-source Firmware SDK (Zephyr RTOS, nRF Connect SDK, ESP-IDF, ModusToolbox, Linux) with a REST Management API at api.golioth.io, a web console, and services for OTA firmware updates, device settings, remote procedure calls (RPC), structured time-series data (LightDB Stream), key/value device state (LightDB State), logs, location, and a Pipelines data-routing engine that forwards device data to downstream cloud services. Authentication to the Management API is via project-scoped API keys passed in the x-api-key header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/apis.yml)

## Tags

- IoT
- Device Management
- Firmware
- Zephyr
- OTA
- Embedded
- Connectivity

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-25

## APIs

### Golioth Management API

REST API for managing Golioth projects, devices, credentials, blueprints, tags, settings, OTA firmware artifacts and releases, RPC, logs, and Pipelines. Documented with an OpenAPI 3 definition served by the API itself. Authenticated with a project-scoped API key in the x-api-key header.

- **Human URL:** [https://docs.golioth.io/reference/management-api/](https://docs.golioth.io/reference/management-api/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Device Management
- Projects
- REST

#### Properties

- [Documentation](https://docs.golioth.io/reference/management-api/)
- [OpenAPI](openapi/golioth-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://api.golioth.io/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Swagger](https://api.golioth.io/swagger.json)
- [Authentication](https://docs.golioth.io/reference/management-api/auth)
- [JSON Schema](json-schema/golioth-device-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/golioth-release-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/golioth-stream-record-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/golioth-device-structure.json)
- [JSON Structure](json-structure/golioth-release-structure.json)
- [JSON-LD](json-ld/golioth-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Ruleset](rules/golioth-rules.yml)
- [Example](examples/golioth-create-device-example.json)
- [Example](examples/golioth-create-release-example.json)
- [Example](examples/golioth-invoke-rpc-example.json)
- [Example](examples/golioth-query-stream-example.json)
- [Example](examples/golioth-create-pipeline-example.json)
- [Plans](plans/golioth-plans-pricing.yml)
- [Rate Limits](rate-limits/golioth-rate-limits.yml)
- [Fin Ops](finops/golioth-finops.yml)
- [Vocabulary](vocabulary/golioth-vocabulary.yml)

### Golioth LightDB State

Per-device key/value state store. Devices and cloud services read and write structured state (JSON/CBOR) that is synchronized between device and cloud over CoAP.

- **Human URL:** [https://docs.golioth.io/application-services/lightdb/](https://docs.golioth.io/application-services/lightdb/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- LightDB
- State
- Device Data

#### Properties

- [Documentation](https://docs.golioth.io/application-services/lightdb/)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth LightDB Stream

Time-series ingest endpoint for streaming sensor and telemetry data from devices. Stored data can be queried and routed downstream via Pipelines.

- **Human URL:** [https://docs.golioth.io/application-services/stream/](https://docs.golioth.io/application-services/stream/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Time Series
- Telemetry
- Stream

#### Properties

- [Documentation](https://docs.golioth.io/application-services/stream/)
- [JSON Schema](json-schema/golioth-stream-record-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/golioth-query-stream-example.json)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Remote Procedure Call (RPC)

Bidirectional remote-procedure-call service. The cloud invokes device-side methods registered by firmware and receives the response, enabling on-demand diagnostics and control.

- **Human URL:** [https://docs.golioth.io/device-management/rpc/](https://docs.golioth.io/device-management/rpc/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- RPC
- Device Management
- Control

#### Properties

- [Documentation](https://docs.golioth.io/device-management/rpc/)
- [Example](examples/golioth-invoke-rpc-example.json)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth OTA Firmware Updates

Over-the-air firmware update service. Upload artifacts, group them into releases, target devices by tag or blueprint, and roll out updates with progress tracking and rollback.

- **Human URL:** [https://docs.golioth.io/device-management/ota/](https://docs.golioth.io/device-management/ota/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- OTA
- Firmware
- Updates

#### Properties

- [Documentation](https://docs.golioth.io/device-management/ota/)
- [JSON Schema](json-schema/golioth-release-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/golioth-release-structure.json)
- [Example](examples/golioth-create-release-example.json)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Device Settings

Cloud-managed settings pushed to one device, a group, or an entire fleet. Firmware subscribes to settings keys and receives updates without requiring a firmware release.

- **Human URL:** [https://docs.golioth.io/device-management/settings/](https://docs.golioth.io/device-management/settings/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Settings
- Configuration
- Fleet

#### Properties

- [Documentation](https://docs.golioth.io/device-management/settings/)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Logging

Centralized device logging. Firmware emits structured log lines that are collected, indexed, and made queryable via the console and API.

- **Human URL:** [https://docs.golioth.io/device-management/logging/](https://docs.golioth.io/device-management/logging/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Logs
- Observability

#### Properties

- [Documentation](https://docs.golioth.io/device-management/logging/)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Pipelines

Data routing and transformation engine. Pipelines describe how data arriving from devices is filtered, transformed, and forwarded to downstream destinations such as AWS S3, GCP Pub/Sub, Azure Event Hubs, InfluxDB, MongoDB, and generic webhooks.

- **Human URL:** [https://docs.golioth.io/data-routing/](https://docs.golioth.io/data-routing/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Pipelines
- Data Routing
- Integration

#### Properties

- [Documentation](https://docs.golioth.io/data-routing/)
- [Example](examples/golioth-create-pipeline-example.json)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Location

Location service that resolves device position from cellular tower and Wi-Fi access-point observations submitted by firmware, returning latitude/longitude back to the device or downstream system.

- **Human URL:** [https://docs.golioth.io/application-services/location/](https://docs.golioth.io/application-services/location/)
- **Base URL:** `https://api.golioth.io`

#### Tags

- Location
- Geolocation
- Cellular
- WiFi

#### Properties

- [Documentation](https://docs.golioth.io/application-services/location/)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Firmware SDK

Open-source firmware SDK that connects embedded devices to the Golioth cloud over CoAP. Supports Zephyr RTOS, nRF Connect SDK, ESP-IDF, and ModusToolbox. Implements client APIs for LightDB State, LightDB Stream, RPC, settings, logging, and OTA.

- **Human URL:** [https://github.com/golioth/golioth-firmware-sdk](https://github.com/golioth/golioth-firmware-sdk)
- **Base URL:** `https://github.com/golioth/golioth-firmware-sdk`

#### Tags

- SDK
- Firmware
- Zephyr
- ESP-IDF

#### Properties

- [Repository](https://github.com/golioth/golioth-firmware-sdk)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Python Tools

Python tooling that wraps the Management API for scripting, automation, and CLI-driven workflows against Golioth projects.

- **Human URL:** [https://github.com/golioth/python-golioth-tools](https://github.com/golioth/python-golioth-tools)
- **Base URL:** `https://github.com/golioth/python-golioth-tools`

#### Tags

- SDK
- Python
- CLI

#### Properties

- [Repository](https://github.com/golioth/python-golioth-tools)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth tinymcp

Open-source implementation of the Model Context Protocol (MCP) for resource-constrained embedded devices, enabling large language models to observe and control firmware via MCP tools.

- **Human URL:** [https://github.com/golioth/tinymcp](https://github.com/golioth/tinymcp)
- **Base URL:** `https://github.com/golioth/tinymcp`

#### Tags

- MCP
- AI
- Embedded

#### Properties

- [Repository](https://github.com/golioth/tinymcp)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Golioth Pouch

Non-IP device-to-cloud transport protocol from Golioth, with a companion Bluetooth gateway reference implementation (pouch-gateway) for relaying pouch traffic to the Golioth cloud.

- **Human URL:** [https://github.com/golioth/pouch](https://github.com/golioth/pouch)
- **Base URL:** `https://github.com/golioth/pouch`

#### Tags

- Protocol
- Bluetooth
- Gateway

#### Properties

- [Repository](https://github.com/golioth/pouch)
- [Postman Collection](collections/golioth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/golioth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://golioth.io/)
- [Documentation](https://docs.golioth.io/)
- [Git Hub](https://github.com/golioth)
- [Console](https://console.golioth.io/)
- [Forum](https://forum.golioth.io/)
- [Blog](https://blog.golioth.io/)
- [Training](https://training.golioth.io/)
- [Reference Designs](https://projects.golioth.io/)
- [Pricing](https://golioth.io/pricing)
- [LinkedIn](https://www.linkedin.com/company/golioth/)
- [L L Ms Txt](https://docs.golioth.io/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
