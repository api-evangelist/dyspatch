# Dyspatch

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

Dyspatch is an email template management and production platform that lets marketing, design, and engineering teams build, collaborate on, approve, localize, and publish transactional and marketing messages without hand-coding HTML. Content is authored in DML (Dyspatch Markup Language) using a modular, no-code drag-and-drop builder with reusable blocks and themes, then published to any ESP (Salesforce, HubSpot, Braze, Marketo, and others). Dyspatch also covers SMS, push, voice, and Live Activity messages, AMP for Email, and large-scale localization across hundreds of languages. The public REST API at api.dyspatch.io exposes published templates, drafts with an approval workflow, localizations and translations, customer profiles, themes, blocks, and tags, and is versioned by date through the Accept header. Dyspatch ships official OpenAPI-generated SDKs for six languages, a published MCP server, webhooks, and Agent Skills. Dyspatch is backed by Y Combinator.

**Areas:** Company · Email · Email Templates · Marketing · Messaging · SMS · Push Notifications · Localization · Content Management · Developer Tools

## Dyspatch on APIs.io

Everything profiled for Dyspatch is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/dyspatch/](https://apis.io/providers/dyspatch/)** — or go straight to one of the APIs or properties below.

### APIs (20)

- [Dyspatch Blocks API](https://apis.io/apis/dyspatch/dyspatch-blocks-api/) — The Blocks API from Dyspatch — 6 operation(s) for blocks.
- [Dyspatch Customer Profiles API](https://apis.io/apis/dyspatch/dyspatch-customer-profiles-api/) — Customer Profiles contain JSON data that can be used for template personalization. Each profile can be associated with one or more workspaces, or none, and…
- [Dyspatch Drafts API](https://apis.io/apis/dyspatch/dyspatch-drafts-api/) — Drafts represent unpublished versions of templates that are still mutable. There could be many in progress drafts for a template.
- [Dyspatch Live Activity Drafts API](https://apis.io/apis/dyspatch/dyspatch-live-activity-drafts-api/) — Live Activity Drafts represent unpublished versions of templates that are still mutable. There could be many in progress drafts for a template.
- [Dyspatch Live Activity Localizations API](https://apis.io/apis/dyspatch/dyspatch-live-activity-localizations-api/) — Live Activity Localization objects are the same as Template objects except they contain localized content. If your account is using localizations then use…
- [Dyspatch Live Activity Templates API](https://apis.io/apis/dyspatch/dyspatch-live-activity-templates-api/) — Live Activity Templates are the Live Activity templates found in your Dyspatch account. Only the published Template Draft is returned. A typical integration…
- [Dyspatch Localizations API](https://apis.io/apis/dyspatch/dyspatch-localizations-api/) — Localization objects are the same as Template objects except they contain localized content. If your account is using localizations then use this instead of…
- [Dyspatch Push Drafts API](https://apis.io/apis/dyspatch/dyspatch-push-drafts-api/) — Push Drafts represent unpublished versions of templates that are still mutable. There could be many in progress drafts for a template.
- [Dyspatch Push Localizations API](https://apis.io/apis/dyspatch/dyspatch-push-localizations-api/) — Push Localization objects are the same as Template objects except they contain localized content. If your account is using localizations then use this…
- [Dyspatch Push Templates API](https://apis.io/apis/dyspatch/dyspatch-push-templates-api/) — Push Templates are the Push templates found in your Dyspatch account. Only the published Template Draft is returned. A typical integration will start with…
- [Dyspatch SMS Drafts API](https://apis.io/apis/dyspatch/dyspatch-sms-drafts-api/) — SMS Drafts represent unpublished versions of templates that are still mutable. There could be many in progress drafts for a template.
- [Dyspatch SMS Localizations API](https://apis.io/apis/dyspatch/dyspatch-sms-localizations-api/) — SMS Localization objects are the same as Template objects except they contain localized content. If your account is using localizations then use this…
- [Dyspatch SMS Templates API](https://apis.io/apis/dyspatch/dyspatch-sms-templates-api/) — SMS Templates are the SMS templates found in your Dyspatch account. Only the published Template Draft is returned. A typical integration will start with…
- [Dyspatch Tags API](https://apis.io/apis/dyspatch/dyspatch-tags-api/) — Tags are a way of categorizing your resources (template and drafts) with helpful identifying information. You can decide what tags are useful for you,…
- [Dyspatch Templates API](https://apis.io/apis/dyspatch/dyspatch-templates-api/) — Templates are the email templates found in your Dyspatch account. Only the published Template Draft is returned. A typical integration will start with using…
- [Dyspatch Themes API](https://apis.io/apis/dyspatch/dyspatch-themes-api/) — The Themes API from Dyspatch — 2 operation(s) for themes.
- [Dyspatch Voice Drafts API](https://apis.io/apis/dyspatch/dyspatch-voice-drafts-api/) — Voice Drafts represent unpublished versions of templates that are still mutable. There could be many in progress drafts for a template.
- [Dyspatch Voice Localizations API](https://apis.io/apis/dyspatch/dyspatch-voice-localizations-api/) — Voice Localization objects are the same as Template objects except they contain localized content. If your account is using localizations then use this…
- [Dyspatch Voice Templates API](https://apis.io/apis/dyspatch/dyspatch-voice-templates-api/) — Voice Templates are the Voice templates found in your Dyspatch account. Only the published Template Draft is returned. A typical integration will start with…
- [Dyspatch Workspaces API](https://apis.io/apis/dyspatch/dyspatch-workspaces-api/) — The Workspaces API from Dyspatch — 2 operation(s) for workspaces.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Dyspatch Webhooks](https://apis.io/asyncapis/dyspatch/dyspatch-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [dyspatch](https://apis.io/servers/dyspatch/dyspatch/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Dyspatch Agentic Access](https://apis.io/agentic-access/dyspatch/dyspatch-agentic-access/)

#### Collections (20)

Postman and Open Collection request collections.

- [Dyspatch Blocks API](https://apis.io/collections/dyspatch/open-dyspatch-blocks-api/)
- [Dyspatch Blocks Customer Profiles API](https://apis.io/collections/dyspatch/open-dyspatch-customer-profiles-api/)
- [Dyspatch Blocks Drafts API](https://apis.io/collections/dyspatch/open-dyspatch-drafts-api/)
- [Dyspatch Blocks Live Activity Drafts API](https://apis.io/collections/dyspatch/open-dyspatch-live-activity-drafts-api/)
- [Dyspatch Blocks Live Activity Localizations API](https://apis.io/collections/dyspatch/open-dyspatch-live-activity-localizations-api/)
- [Dyspatch Blocks Live Activity Templates API](https://apis.io/collections/dyspatch/open-dyspatch-live-activity-templates-api/)
- [Dyspatch Blocks Localizations API](https://apis.io/collections/dyspatch/open-dyspatch-localizations-api/)
- [Dyspatch Blocks Push Drafts API](https://apis.io/collections/dyspatch/open-dyspatch-push-drafts-api/)
- [Dyspatch Blocks Push Localizations API](https://apis.io/collections/dyspatch/open-dyspatch-push-localizations-api/)
- [Dyspatch Blocks Push Templates API](https://apis.io/collections/dyspatch/open-dyspatch-push-templates-api/)
- [Dyspatch Blocks SMS Drafts API](https://apis.io/collections/dyspatch/open-dyspatch-sms-drafts-api/)
- [Dyspatch Blocks SMS Localizations API](https://apis.io/collections/dyspatch/open-dyspatch-sms-localizations-api/)
- [Dyspatch Blocks SMS Templates API](https://apis.io/collections/dyspatch/open-dyspatch-sms-templates-api/)
- [Dyspatch Blocks Tags API](https://apis.io/collections/dyspatch/open-dyspatch-tags-api/)
- [Dyspatch Blocks Templates API](https://apis.io/collections/dyspatch/open-dyspatch-templates-api/)
- [Dyspatch Blocks Themes API](https://apis.io/collections/dyspatch/open-dyspatch-themes-api/)
- [Dyspatch Blocks Voice Drafts API](https://apis.io/collections/dyspatch/open-dyspatch-voice-drafts-api/)
- [Dyspatch Blocks Voice Localizations API](https://apis.io/collections/dyspatch/open-dyspatch-voice-localizations-api/)
- [Dyspatch Blocks Voice Templates API](https://apis.io/collections/dyspatch/open-dyspatch-voice-templates-api/)
- [Dyspatch Blocks Workspaces API](https://apis.io/collections/dyspatch/open-dyspatch-workspaces-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Dyspatch Openapi Overlay](https://apis.io/overlays/dyspatch/dyspatch-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Dyspatch Authentication](https://apis.io/security/dyspatch/dyspatch-authentication/)
- [Dyspatch Domain Security](https://apis.io/security/dyspatch/dyspatch-domain-security/)
- [Dyspatch Vulnerability Disclosure](https://apis.io/security/dyspatch/dyspatch-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Dyspatch Plans Pricing](https://apis.io/plans/dyspatch/dyspatch-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Dyspatch Rate Limits](https://apis.io/rate-limits/dyspatch/dyspatch-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.dyspatch.io/)
- [Documentation](https://docs.dyspatch.io)
- [Getting started](https://docs.dyspatch.io/administration/creating_api_keys/)
- [API reference](https://docs.dyspatch.io/api/)
- [Pricing](https://www.dyspatch.io/pricing/)
- [Sign up](https://app.dyspatch.io/)
- [Support](https://docs.dyspatch.io)
- [Blog](https://www.dyspatch.io/blog/)
- [Terms of service](https://www.dyspatch.io/terms-of-service/)
- [Privacy policy](https://www.dyspatch.io/privacy-policy/)
- [GitHub](https://github.com/getdyspatch)
- [Status](https://status.dyspatch.io)

## API Evangelist rating

**Kin Score 58.5** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 62.3 |
| Contract governance | 4.5 |
| Operational transparency | 52.6 |
| Developer ergonomics | 67.3 |
| Access clarity | 63.2 |

**Agent readiness 36.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 25.8** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/dyspatch/](https://apis.io/providers/dyspatch/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Dyspatch: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/dyspatch/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
