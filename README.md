# Waste Management

Waste Management (WM) is the largest environmental services company in North America, providing waste collection, transfer, disposal, and recycling services to over 20 million residential, commercial, industrial, and municipal customers. WM provides RESTful APIs for customers and third-party integrators to access account data including balance, services, invoices, pickup schedules, and ETAs via JWT authentication.

**Website:** https://www.wm.com  
**API Portal:** https://api.wm.com/  
**APIs.json:** https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/apis.yml

## Tags

Environmental Services, Fortune 500, Recycling, Solid Waste, Sustainability, Waste Management

---

## APIs

### Waste Management Customer API

RESTful API providing access to customer account data including balance due, contract details, invoice history, service details, pickup schedules, ETAs, contacts, and preferences. Requires JWT bearer authentication plus ClientId and Request-Tracking-Id headers.

- **Documentation:** https://api.wm.com/
- **OpenAPI:** [openapi/waste-management-customer-api-openapi.yml](openapi/waste-management-customer-api-openapi.yml)

---

## Artifacts

### OpenAPI Specifications

| File | Description |
|------|-------------|
| [openapi/waste-management-customer-api-openapi.yml](openapi/waste-management-customer-api-openapi.yml) | Full Customer API covering account, services, invoices, contacts, preferences, and ETAs |

### Spectral Rules

| File | Description |
|------|-------------|
| [rules/waste-management-rules.yml](rules/waste-management-rules.yml) | Spectral ruleset enforcing WM API conventions: required headers, bearer auth, HTTPS, Title Case summaries |

### Naftiko Capabilities

| File | Description |
|------|-------------|
| [capabilities/customer-service.yaml](capabilities/customer-service.yaml) | Unified customer service workflow — 14 MCP tools covering account, services, pickup, billing, and preferences |
| [capabilities/shared/customer-api.yaml](capabilities/shared/customer-api.yaml) | Shared per-API definition for the WM Customer API |

### JSON Schemas

| File | Description |
|------|-------------|
| [json-schema/waste-management-service-schema.json](json-schema/waste-management-service-schema.json) | Service record schema with material, equipment, and pricing fields |
| [json-schema/waste-management-invoice-schema.json](json-schema/waste-management-invoice-schema.json) | Invoice schema with line items and fee types |

### JSON Structures

| File | Description |
|------|-------------|
| [json-structure/waste-management-service-structure.json](json-structure/waste-management-service-structure.json) | Service field structure documentation |

### JSON-LD Contexts

| File | Description |
|------|-------------|
| [json-ld/waste-management-context.jsonld](json-ld/waste-management-context.jsonld) | JSON-LD context mapping WM API fields to schema.org |

### Examples

| File | Description |
|------|-------------|
| [examples/waste-management-getCustomerOverview-example.json](examples/waste-management-getCustomerOverview-example.json) | Get Customer Overview request/response |
| [examples/waste-management-listServices-example.json](examples/waste-management-listServices-example.json) | List Services request/response |
| [examples/waste-management-listInvoices-example.json](examples/waste-management-listInvoices-example.json) | List Invoices request/response with date filtering |
| [examples/waste-management-getServiceEta-example.json](examples/waste-management-getServiceEta-example.json) | Get Service ETA request/response |

### Vocabulary

| File | Description |
|------|-------------|
| [vocabulary/waste-management-vocabulary.yml](vocabulary/waste-management-vocabulary.yml) | Domain vocabulary: Line of Business, Service ETA, Invoice Fee, AutoPay, Material, Request Tracking ID |

---

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
