---
generated: '2026-10-08'
method: generated
name: prove-identity-manager-enroll
description: 'Manage persistent identities in the Prove Identity Manager: enroll by phone number, look up by proveId
  or phone number, page through the batch, and disenroll.'
api: openapi/prove-identity-api-openapi.yml
operations:
- v3EnrollIdentity
- v3GetIdentity
- v3GetIdentitiesByPhoneNumber
- v3BatchGetIdentities
- v3DisenrollIdentity
source: Grounded in openapi/_original/prove-openapi.yml and the Pre-Fill flow order in the prove-postman README;
  operationIds verified in openapi/prove-identity-api-openapi.yml
---

# Enroll, look up and disenroll an identity

Manage persistent identities in the Prove Identity Manager: enroll by phone number, look up by proveId or phone number, page through the batch, and disenroll.

## Auth
- Bearer token from `POST /v3/token` (`v3TokenRequest`, `openapi/prove-authentication-api-openapi.yml`).

## Steps
1. **Enroll** — `v3EnrollIdentity` (`POST /v3/identity`) with `phoneNumber` and optional `clientCustomerId`, `clientHumanId`, `clientRequestId`, `deviceId`, `identityAttributes`. The response is an `Identity` with `proveId` and `state`.
2. **Look up** — `v3GetIdentity` (`GET /v3/identity/{proveId}`) for one record, or `v3GetIdentitiesByPhoneNumber` (`GET /v3/identity/{mobileNumber}/lookup`) to find identities for a phone number.
3. **Page the batch** — `v3BatchGetIdentities` (`GET /v3/identity`) with the `startKey` cursor query parameter to walk all identities.
4. **Disenroll** — `v3DisenrollIdentity` (`DELETE /v3/identity/{proveId}`) to remove an identity.

## Rules
- Disenroll is the reversal of enroll; no retention or restore window is published, so treat it as final. See `conventions/prove-conventions.yml`.
- No idempotency key exists; check for an existing identity with the lookup before enrolling again.
- Errors return `{ code, message, details }`; `404` applies to the by-id reads.
