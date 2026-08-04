# tyntec (tyntec)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

tyntec is a CPaaS (Communications Platform as a Service) provider whose `api.tyntec.com` REST APIs let businesses verify, authenticate, and engage mobile consumers worldwide. The platform covers **phone number verification and number information** (Verify API plus HLR lookup and global number portability), **SMS messaging**, **WhatsApp Business** and other chat-app channels via the Conversations API, and **two-factor authentication / one-time passwords** via the 2FA API. tyntec is an authorized WhatsApp Business Solution Provider.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/apis.yml)

## Access Model

tyntec runs a real, publicly documented API program. The API reference is public at [api.tyntec.com/reference](https://api.tyntec.com/reference/), and tyntec publishes open OpenAPI definitions for every product in the public [tyntec/api-collection](https://github.com/tyntec/api-collection) GitHub repository. To call the APIs you need a tyntec account and an **API key**, which is sent in the `apikey` request header on every request (the Verify reference also names the header `apiKey`; it is case-insensitive). There is no OAuth or Bearer flow. Billing is usage-based (pay-per-use against a prepaid account balance), so live calls incur per-transaction charges.

Asynchronous events - SMS delivery receipts, inbound messages, WhatsApp/Viber status updates - are delivered by **HTTP webhook callbacks** to a URL you configure, not over a WebSocket. See [`review.yml`](review.yml).

> Note on artifacts: endpoint paths, base paths, and the `apikey` auth scheme in this repo are grounded in tyntec's public reference and the tyntec/api-collection specs. The OpenAPI and Postman/Open Collection artifacts in this repo model the **Number Verification + Number Information** surface in detail (the primary use case this entry targets); JSON request/response schemas are honestly modeled from the docs and simplified for cataloging. The SMS, Conversations, and 2FA APIs are cataloged with their live reference and source links.

## Tags

- Number Verification
- CPaaS
- SMS
- WhatsApp
- Phone Number Intelligence
- HLR Lookup
- Two-Factor Authentication
- OTP
- Messaging
- Number Portability

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### tyntec Number Verification API

Verify a phone number before saving it to a CRM, messaging it, or calling it. Define reusable criteria templates (allowed line types, countries, reachable subscriber required, reject disposable numbers) and validate any number against them, returning validity, active-subscriber reachability, line type, operator, country of origin, MCC/MNC, and disposable-number detection.

- **Human URL:** [https://api.tyntec.com/reference/verify/current.html](https://api.tyntec.com/reference/verify/current.html)
- **Base URL:** `https://api.tyntec.com/verify/v1`

#### Tags

- Number Verification
- Phone Number Intelligence
- Validation

#### Properties

- [Documentation](https://www.tyntec.com/helpcenter/docs/)
- [API Reference](https://api.tyntec.com/reference/verify/current.html)
- [OpenAPI](openapi/tyntec-number-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyntec-number-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tyntec-number-verification.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Source Code](https://github.com/tyntec/api-collection/tree/master/verify)

### tyntec Number Information API

Network-grade number intelligence. HLR (Home Location Register) lookup via `GNV` returns real-time subscriber reachability, roaming state, and serving / original operator; Global Number Portability (`GNP`) resolves whether a number has been ported and to which operator, for correct message and call routing.

- **Human URL:** [https://api.tyntec.com/reference/verify/current.html](https://api.tyntec.com/reference/verify/current.html)
- **Base URL:** `https://api.tyntec.com/nis/v1`

#### Tags

- HLR Lookup
- Number Portability
- Phone Number Intelligence

#### Properties

- [Documentation](https://www.tyntec.com/helpcenter/docs/)
- [API Reference](https://api.tyntec.com/reference/verify/current.html)
- [OpenAPI](openapi/tyntec-number-verification-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyntec-number-verification.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Source Code](https://github.com/tyntec/api-collection/tree/master/verify)

### tyntec 2FA Authentication API

Programmatic two-factor authentication and one-time passwords. Send an OTP to a recipient number (`POST /otp`), validate the code the user enters (`POST /otp/{otp-id}/validate` returning VERIFIED, EXPIRED, WRONG_CODE, or TOO_MANY_ATTEMPTS), and read, list, or delete OTP records.

- **Human URL:** [https://api.tyntec.com/reference/otp-authentication/current.html](https://api.tyntec.com/reference/otp-authentication/current.html)
- **Base URL:** `https://api.tyntec.com/2fa/v4`

#### Tags

- Two-Factor Authentication
- OTP
- Number Verification

#### Properties

- [Documentation](https://www.tyntec.com/helpcenter/docs/)
- [API Reference](https://api.tyntec.com/reference/otp-authentication/current.html)
- [Source Code](https://github.com/tyntec/api-collection/tree/master/otp-authentication)

### tyntec SMS API

Send and receive text messages over tyntec's global A2P SMS network. Send via `POST /messaging/v1/sms`, retrieve delivery status via `GET /messaging/v1/messages/{requestId}`, receive inbound SMS by webhook, and report delivery conversion events. Includes BYON (bring your own number) contact, phone book, and number provisioning services.

- **Human URL:** [https://api.tyntec.com/reference/sms/current.html](https://api.tyntec.com/reference/sms/current.html)
- **Base URL:** `https://api.tyntec.com/messaging/v1`

#### Tags

- SMS
- Messaging
- A2P

#### Properties

- [Documentation](https://www.tyntec.com/helpcenter/docs/)
- [API Reference](https://api.tyntec.com/reference/sms/current.html)
- [Source Code](https://github.com/tyntec/api-collection/tree/master/sms)

### tyntec Conversations API

One API for WhatsApp Business, Viber, and SMS. Send single (`POST /messages`) or bulk (`POST /bulks`) messages, track delivery status and events, upload and manage media, configure WhatsApp accounts / templates / phone-number insights, and receive inbound messages and status callbacks via webhooks. tyntec is an authorized WhatsApp Business Solution Provider.

- **Human URL:** [https://api.tyntec.com/reference/conversations/current.html](https://api.tyntec.com/reference/conversations/current.html)
- **Base URL:** `https://api.tyntec.com/conversations/v3`

#### Tags

- WhatsApp
- Messaging
- Chat Apps

#### Properties

- [Documentation](https://www.tyntec.com/helpcenter/docs/channels/whatsapp-business/introduction/)
- [API Reference](https://api.tyntec.com/reference/conversations/current.html)
- [Source Code](https://github.com/tyntec/api-collection/tree/master/conversations)

## Common Properties

- [Domain Security](security/tyntec-domain-security.yml)
- [Authentication](authentication/tyntec-authentication.yml)
- [GitHub Organization](https://github.com/tyntec)
- [LinkedIn](https://www.linkedin.com/company/tyntec)
- [Website](https://www.tyntec.com)
- [Documentation](https://api.tyntec.com/reference/)
- [Plans](plans/tyntec-plans-pricing.yml)
- [Rate Limits](rate-limits/tyntec-rate-limits.yml)
- [Fin Ops](finops/tyntec-finops.yml)
- [Blog](https://www.tyntec.com/blog)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
