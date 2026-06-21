# Prove (prove)

Prove is a phone-centric digital identity verification and authentication platform. The Prove API (v3) uses the consumer's mobile phone number and cryptographic possession signals to power Pre-Fill identity prefill, passive Trust Score verification, Unified Authentication, and an Identity Manager - all behind an OAuth 2.0 secured REST interface at https://api.prove.com/v3.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/apis.yml)

## Tags

- Identity Verification
- Authentication
- Phone Intelligence
- KYC
- Fraud Prevention

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Prove Identity Verification (v3 Flows)

The ordered Pre-Fill verification flow - start, validate, challenge, and complete - that initiates a session against a mobile phone number, confirms possession, optionally challenges with DOB/SSN, and returns reconciled, prefilled identity attributes plus IDV/KYC evaluation.

- **Human URL:** [https://developer.prove.com/docs/prove-pre-fill-flow](https://developer.prove.com/docs/prove-pre-fill-flow)
- **Base URL:** `https://api.prove.com/v3`

#### Tags

- Identity Verification
- Pre-Fill
- OTP
- KYC

#### Properties

- [Documentation](https://developer.prove.com/docs/prove-pre-fill-flow)
- [API Reference](https://developer.prove.com/reference/start-request)
- [OpenAPI](openapi/prove-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prove.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prove.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Prove Trust Score (Unified Authentication)

Unified Authentication (Unify) flow - unify, unify-bind, and unify-status - that passively recognizes a returning customer by phone possession and a bound Prove Key, returning a real-time trust and possession evaluation for risk-aware decisions.

- **Human URL:** [https://developer.prove.com/reference/unify-server](https://developer.prove.com/reference/unify-server)
- **Base URL:** `https://api.prove.com/v3`

#### Tags

- Trust Score
- Authentication
- Possession
- Risk

#### Properties

- [Documentation](https://developer.prove.com/reference/unify-server)
- [OpenAPI](openapi/prove-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prove.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prove.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Prove Pre-Fill (Identity Discovery)

Identity discovery and attribute retrieval - discover and fetch - that surface which verified identity attributes Prove can return for a phone number and then fetch the authoritative attribute values to prefill onboarding forms.

- **Human URL:** [https://developer.prove.com/reference/prefill-identity-server](https://developer.prove.com/reference/prefill-identity-server)
- **Base URL:** `https://api.prove.com/v3`

#### Tags

- Pre-Fill
- Identity Discovery
- Onboarding

#### Properties

- [Documentation](https://developer.prove.com/reference/prefill-identity-server)
- [OpenAPI](openapi/prove-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prove.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prove.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Prove Auth

Phone-based authentication - auth start, continue, and finish, plus device revoke - that authenticates a known customer via mobile possession and cryptographic device binding for step-up and ongoing authentication.

- **Human URL:** [https://developer.prove.com/reference/unify-server](https://developer.prove.com/reference/unify-server)
- **Base URL:** `https://api.prove.com/v3`

#### Tags

- Authentication
- Phone Auth
- Device Binding

#### Properties

- [Documentation](https://developer.prove.com/reference/unify-server)
- [OpenAPI](openapi/prove-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prove.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prove.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Prove Identity Manager

Identity lifecycle management - enroll, batch enroll, get, lookup by phone number, cross-domain, and disenroll - that maintains a persistent customer identity record keyed to a phone number for recognition across sessions and domains.

- **Human URL:** [https://developer.prove.com/reference/prefill-identity-server](https://developer.prove.com/reference/prefill-identity-server)
- **Base URL:** `https://api.prove.com/v3`

#### Tags

- Identity
- Enrollment
- Lifecycle

#### Properties

- [Documentation](https://developer.prove.com/reference/prefill-identity-server)
- [OpenAPI](openapi/prove-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prove.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prove.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/prove-identity)
- [LinkedIn](https://www.linkedin.com/company/proveidentity)
- [Website](https://www.prove.com)
- [Documentation](https://developer.prove.com)
- [Plans](plans/prove-plans-pricing.yml)
- [Rate Limits](rate-limits/prove-rate-limits.yml)
- [Fin Ops](finops/prove-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
