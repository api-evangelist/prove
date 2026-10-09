---
generated: '2026-10-08'
method: generated
name: prove-unified-authentication
description: Run a Unified Authentication session for a phone number, bind a Prove Key if requested, and read the
  possession result and trust evaluation.
api: openapi/prove-trust-score-api-openapi.yml
operations:
- v3UnifyRequest
- v3UnifyBindRequest
- v3UnifyStatusRequest
source: Grounded in openapi/_original/prove-openapi.yml and the Pre-Fill flow order in the prove-postman README;
  operationIds verified in openapi/prove-trust-score-api-openapi.yml
---

# Authenticate a user with Unify (Trust Score)

Run a Unified Authentication session for a phone number, bind a Prove Key if requested, and read the possession result and trust evaluation.

## Auth
- Bearer token from `POST /v3/token` (`v3TokenRequest`, `openapi/prove-authentication-api-openapi.yml`). See `authentication/prove-authentication.yml`.

## Steps
1. **Start the session** — `v3UnifyRequest` (`POST /v3/unify`) with `phoneNumber`; optional `possessionType`, `finalTargetURL`, `clientCustomerId`, `clientHumanId`, `clientRequestId`, `deviceId`, `proveId`, `rebind`, `checkReputation`, `allowOTPRetry`. Keep `correlationId`; follow `next`.
2. **Bind (when `next` offers it)** — `v3UnifyBindRequest` (`POST /v3/unify-bind`) with `correlationId` to bind a Prove Key to the session.
3. **Read the result** — `v3UnifyStatusRequest` (`POST /v3/unify-status`) with `correlationId`; the response carries `possessionResult` and `evaluation`.

## Rules
- Pass your own `clientRequestId` for your audit trail; it is not a replay-protection key (`idempotency.coverage: none`).
- A device bound through this flow can later be revoked with `v3DeviceRevokeRequest` in `openapi/prove-auth-api-openapi.yml`; no time window is stated. See `conventions/prove-conventions.yml` reversibility.
