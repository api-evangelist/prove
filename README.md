# Prove

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

Prove is a phone-centric digital identity verification and authentication platform. The Prove API (v3) uses the consumer's mobile phone number and cryptographic possession signals to power Pre-Fill identity prefill, passive Trust Score verification, Unified Authentication, phone-based Auth and a persistent Identity Manager - all behind an OAuth 2.0 client-credentials REST interface served from regional hosts (https://platform.proveapis.com/v3 for the US, https://platform.eu.proveapis.com/v3 for the EU, with UAT sandboxes for each). Official server SDKs ship for TypeScript, Go, Java and .NET, plus web and mobile Auth client SDKs and a public Postman workspace.

**Areas:** Identity Verification · Authentication · Phone Intelligence · KYC · Fraud Prevention

## Prove on APIs.io

Everything profiled for Prove is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/prove/](https://apis.io/providers/prove/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Prove Auth API](https://apis.io/apis/prove/prove-auth-api/) — Phone-based authentication and device binding.
- [Prove Authentication API](https://apis.io/apis/prove/prove-authentication-api/) — OAuth 2.0 token issuance.
- [Prove Domain API](https://apis.io/apis/prove/prove-domain-api/) — Cross-domain linking of identity scopes.
- [Prove Identity API](https://apis.io/apis/prove/prove-identity-api/) — Persistent identity lifecycle management.
- [Prove Identity Verification API](https://apis.io/apis/prove/prove-identity-verification-api/) — Ordered Pre-Fill verification flow - start, validate, challenge, complete.
- [Prove Pre-Fill API](https://apis.io/apis/prove/prove-pre-fill-api/) — Identity discovery and verified attribute retrieval.
- [Prove Trust Score API](https://apis.io/apis/prove/prove-trust-score-api/) — Unified Authentication possession and trust evaluation.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [prove-docs](https://apis.io/servers/prove/prove-docs/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Prove Agentic Access](https://apis.io/agentic-access/prove/prove-agentic-access/)

#### JSON Schema (21)

The data models the API reads and writes.

- [AuthContinueRequest](https://apis.io/schemas/prove/prove-auth-continue-request/)
- [AuthResponse](https://apis.io/schemas/prove/prove-auth-response/)
- [AuthStartRequest](https://apis.io/schemas/prove/prove-auth-start-request/)
- [DeviceRevokeRequest](https://apis.io/schemas/prove/prove-device-revoke-request/)
- [DiscoverResponse](https://apis.io/schemas/prove/prove-discover-response/)
- [EnrollIdentityRequest](https://apis.io/schemas/prove/prove-enroll-identity-request/)
- [FetchResponse](https://apis.io/schemas/prove/prove-fetch-response/)
- [Identity](https://apis.io/schemas/prove/prove-identity/)
- [IdentityListResponse](https://apis.io/schemas/prove/prove-identity-list-response/)
- [SuccessResponse](https://apis.io/schemas/prove/prove-success-response/)
- [TokenRequest](https://apis.io/schemas/prove/prove-token-request/)
- [TokenResponse](https://apis.io/schemas/prove/prove-token-response/)
- [V3ChallengeRequest](https://apis.io/schemas/prove/prove-v3-challenge-request/)
- [V3CompleteRequest](https://apis.io/schemas/prove/prove-v3-complete-request/)
- [V3CompleteResponse](https://apis.io/schemas/prove/prove-v3-complete-response/)
- [V3CorrelationRequest](https://apis.io/schemas/prove/prove-v3-correlation-request/)
- [V3FlowResponse](https://apis.io/schemas/prove/prove-v3-flow-response/)
- [V3StartRequest](https://apis.io/schemas/prove/prove-v3-start-request/)
- [V3StartResponse](https://apis.io/schemas/prove/prove-v3-start-response/)
- [V3UnifyRequest](https://apis.io/schemas/prove/prove-v3-unify-request/)
- [V3UnifyStatusResponse](https://apis.io/schemas/prove/prove-v3-unify-status-response/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Prove Context](https://apis.io/jsonld/prove/prove-context/)

#### Collections (8)

Postman and Open Collection request collections.

- [Prove API](https://apis.io/collections/prove/open-prove/)
- [Prove Auth API](https://apis.io/collections/prove/open-prove-auth-api/)
- [Prove Auth Authentication API](https://apis.io/collections/prove/open-prove-authentication-api/)
- [Prove Auth Domain API](https://apis.io/collections/prove/open-prove-domain-api/)
- [Prove Auth Identity API](https://apis.io/collections/prove/open-prove-identity-api/)
- [Prove Auth Identity Verification API](https://apis.io/collections/prove/open-prove-identity-verification-api/)
- [Prove Auth Pre-Fill API](https://apis.io/collections/prove/open-prove-pre-fill-api/)
- [Prove Auth Trust Score API](https://apis.io/collections/prove/open-prove-trust-score-api/)

#### Overlays (7)

OpenAPI overlays, including conversational phrasing for each operation.

- [Prove Auth Api Overlay](https://apis.io/overlays/prove/prove-auth-api-overlay/)
- [Prove Authentication Api Overlay](https://apis.io/overlays/prove/prove-authentication-api-overlay/)
- [Prove Domain Api Overlay](https://apis.io/overlays/prove/prove-domain-api-overlay/)
- [Prove Identity Api Overlay](https://apis.io/overlays/prove/prove-identity-api-overlay/)
- [Prove Identity Verification Api Overlay](https://apis.io/overlays/prove/prove-identity-verification-api-overlay/)
- [Prove Pre Fill Api Overlay](https://apis.io/overlays/prove/prove-pre-fill-api-overlay/)
- [Prove Trust Score Api Overlay](https://apis.io/overlays/prove/prove-trust-score-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Prove API Rules](https://apis.io/rules/prove/prove-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Prove Authentication](https://apis.io/security/prove/prove-authentication/)
- [Prove Domain Security](https://apis.io/security/prove/prove-domain-security/)
- [Prove Trust Center](https://apis.io/security/prove/prove-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Prove Scopes](https://apis.io/scopes/prove/prove-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Prove Plans Pricing](https://apis.io/plans/prove/prove-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Prove Rate Limits](https://apis.io/rate-limits/prove/prove-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Prove Finops](https://apis.io/finops/prove/prove-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.prove.com)
- [Documentation](https://developer.prove.com)
- [Sign up](https://portal.prove.com/en/signup)
- [Support](https://support.prove.com/s/)
- [Blog](https://www.prove.com/blog)
- [Terms of service](https://www.prove.com/legal/prove-terms-of-service)
- [Privacy policy](https://www.prove.com/legal/overview)
- [GitHub](https://github.com/prove-identity)
- [Status](https://status.prove.com/)

## API Evangelist rating

**Kin Score 51.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 76.7 |
| Contract quality | 62.7 |
| Contract governance | 22.0 |
| Operational transparency | 28.9 |
| Developer ergonomics | 49.4 |
| Access clarity | 42.1 |

**Agent readiness 42.3** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/prove/](https://apis.io/providers/prove/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Prove: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/prove/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
