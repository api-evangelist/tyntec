# tyntec

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

tyntec is a CPaaS (Communications Platform as a Service) provider whose api.tyntec.com REST APIs let businesses verify, authenticate, and engage mobile consumers worldwide. The platform covers phone number verification and number information (Verify API plus HLR lookup and global number portability), SMS messaging, WhatsApp Business and other chat-app channels via the Conversations API, and two-factor authentication / one-time passwords via the 2FA API. tyntec is an authorized WhatsApp Business Solution Provider. All APIs authenticate with an account API key sent in the apikey request header; tyntec publishes OpenAPI definitions for them in the public tyntec/api-collection GitHub repository.

**Areas:** Number Verification · CPaaS · SMS · WhatsApp · Phone Number Intelligence · HLR Lookup · Two-Factor Authentication · OTP · Messaging · Number Portability

## tyntec on APIs.io

Everything profiled for tyntec is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/tyntec/](https://apis.io/providers/tyntec/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [tyntec 2FA Authentication API](https://apis.io/apis/tyntec/tyntec-2fa-authentication-api/) — Programmatic two-factor authentication and one-time passwords. Send an OTP to a recipient number (POST /otp), validate the code the user enters (POST…
- [tyntec SMS API](https://apis.io/apis/tyntec/tyntec-sms-api/) — Send and receive text messages over tyntec's global A2P SMS network. Send via POST /messaging/v1/sms, retrieve delivery status via GET…
- [tyntec Conversations API](https://apis.io/apis/tyntec/tyntec-conversations-api/) — One API for WhatsApp Business, Viber, and SMS. Send single (POST /messages) or bulk (POST /bulks) messages, track delivery status and events, upload and…
- [tyntec Number Information API](https://apis.io/apis/tyntec/tyntec-number-information-api/) — HLR reachability/roaming and global number portability lookups (NIS).
- [tyntec Number Verification API](https://apis.io/apis/tyntec/tyntec-number-verification-api/) — Validate a phone number against reusable criteria templates (Verify API).
- [tyntec Service API](https://apis.io/apis/tyntec/tyntec-service-api/) — Health and version metadata.
- [tyntec Verify Templates API](https://apis.io/apis/tyntec/tyntec-verify-templates-api/) — Create and manage the criteria templates numbers are checked against.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Tyntec Agentic Access](https://apis.io/agentic-access/tyntec/tyntec-agentic-access/)

#### Collections (5)

Postman and Open Collection request collections.

- [tyntec Phone Number Intelligence Number Information API](https://apis.io/collections/tyntec/open-tyntec-number-information-api/)
- [tyntec Phone Number Intelligence API](https://apis.io/collections/tyntec/open-tyntec-number-verification/)
- [tyntec Phone Number Intelligence Number Information Number Verification API](https://apis.io/collections/tyntec/open-tyntec-number-verification-api/)
- [tyntec Phone Number Intelligence Number Information Service API](https://apis.io/collections/tyntec/open-tyntec-service-api/)
- [tyntec Phone Number Intelligence Number Information Verify Templates API](https://apis.io/collections/tyntec/open-tyntec-verify-templates-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Tyntec Authentication](https://apis.io/security/tyntec/tyntec-authentication/)
- [Tyntec Domain Security](https://apis.io/security/tyntec/tyntec-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Tyntec Plans Pricing](https://apis.io/plans/tyntec/tyntec-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Tyntec Rate Limits](https://apis.io/rate-limits/tyntec/tyntec-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Tyntec Finops](https://apis.io/finops/tyntec/tyntec-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.tyntec.com)
- [Documentation](https://api.tyntec.com/reference/)
- [Blog](https://www.tyntec.com/blog)
- [GitHub](https://github.com/tyntec)

## API Evangelist rating

**Kin Score 16.1** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 3.4 |
| Contract governance | 0.0 |
| Operational transparency | 26.3 |
| Developer ergonomics | 32.1 |
| Access clarity | 5.3 |

**Agent readiness 17.9** — agent-aware

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

**Regulatory alignment 10.0** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/tyntec/](https://apis.io/providers/tyntec/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for tyntec: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/tyntec/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
