---
generated: '2026-10-08'
method: generated
name: prove-prefill-verify-identity
description: 'Run the ordered Pre-Fill verification flow for a consumer phone number: start, validate, challenge,
  complete.'
api: openapi/prove-identity-verification-api-openapi.yml
operations:
- v3StartRequest
- v3ValidateRequest
- v3ChallengeRequest
- v3CompleteRequest
source: Grounded in openapi/_original/prove-openapi.yml and the Pre-Fill flow order in the prove-postman README;
  operationIds verified in openapi/prove-identity-verification-api-openapi.yml
---

# Verify an identity with Pre-Fill

Run the ordered Pre-Fill verification flow for a consumer phone number: start, validate, challenge, complete.

## Auth
- Exchange the project Client ID + Client Secret at `POST /v3/token` (`v3TokenRequest`, in `openapi/prove-authentication-api-openapi.yml`) and send the `access_token` as a Bearer token on every call. See `authentication/prove-authentication.yml`.
- Use the UAT host (`https://platform.uat.proveapis.com/v3`) with sandbox credentials first; production is `https://platform.proveapis.com/v3`. See `sandbox/prove-sandbox.yml`.

## Steps
1. **Start** — `v3StartRequest` (`POST /v3/start`) with `flowType` and `phoneNumber` (optional `finalTargetURL`, `emailAddress`, `smsMessage`, `ipAddress`, `dob`, `ssn`, `allowOTPRetry`). Keep the returned `correlationId` and `authToken`; read `next` for the step the server allows.
2. **Validate** — `v3ValidateRequest` (`POST /v3/validate`) with `correlationId` once the consumer has completed the possession check; `success` and `next` tell you whether to challenge.
3. **Challenge** — `v3ChallengeRequest` (`POST /v3/challenge`) with `correlationId` and, when `next` asks for it, `dob` or `ssn`.
4. **Complete** — `v3CompleteRequest` (`POST /v3/complete`) with `correlationId` and the `individual` record the consumer confirmed; read `evaluation`, `idv` and `kyc` in the response.

## Rules
- Call the steps strictly in order and always follow the `next` map; the flow is stateful per `correlationId`. See `conventions/prove-conventions.yml`.
- There is no idempotency key (`idempotency.coverage: none`): do not blindly retry a POST that may have succeeded; re-read `next` instead.
- The flow is an assessment and cannot be reversed; nothing needs undoing if it is abandoned.
- Errors return `{ code, message, details }` with 400/401 (see `errors/prove-problem-types.yml`).
