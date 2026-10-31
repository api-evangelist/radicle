# Radicle

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

Radicle is a sovereign, peer-to-peer code collaboration stack built on Git, developed by Radicle (radicle.dev) and backed by Electric Capital. Instead of relying on a central host, every user runs their own node, and repositories, issues and patches replicate across the network as cryptographically-signed Collaborative Objects (COBs). The stack ships the `rad` command-line tooling, the Heartwood protocol and node, a terminal UI, a desktop app, and a web explorer. Each node can run `radicle-httpd`, a lightweight HTTP daemon that exposes a read-oriented JSON API over the node's storage — repositories, issues, patches, commits, source trees, node info and network statistics — which powers the Radicle web explorer and third-party tooling. Identity is key-based (DIDs / did:key), so there are no accounts, passwords or platform lock-in. This profile was enriched from Radicle's public surface: the live seed node API, the security.txt, the Heartwood source, and the CLI manuals.

**Areas:** Company · Developer Tools · Code Collaboration · Version Control · Peer-to-Peer · Open Source · Decentralized · Developer Tools API

## Radicle on APIs.io

Everything profiled for Radicle is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/radicle/](https://apis.io/providers/radicle/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Radicle Issues API](https://apis.io/apis/radicle/radicle-issues-api/) — Repository issues (collaborative objects)
- [Radicle Node API](https://apis.io/apis/radicle/radicle-node-api/) — Node identity, configuration and peers
- [Radicle Patches API](https://apis.io/apis/radicle/radicle-patches-api/) — Repository patches (change proposals)
- [Radicle Repositories API](https://apis.io/apis/radicle/radicle-repositories-api/) — Radicle repositories seeded by the node
- [Radicle Service API](https://apis.io/apis/radicle/radicle-service-api/) — API root and service metadata
- [Radicle Source API](https://apis.io/apis/radicle/radicle-source-api/) — Commits, trees, blobs and READMEs
- [Radicle Stats API](https://apis.io/apis/radicle/radicle-stats-api/) — Aggregate node statistics

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [radicle](https://apis.io/servers/radicle/radicle/)

#### Collections (7)

Postman and Open Collection request collections.

- [Radicle HTTP API (radicle-httpd) Issues API](https://apis.io/collections/radicle/open-radicle-issues-api/)
- [Radicle HTTP API (radicle-httpd) Issues Node API](https://apis.io/collections/radicle/open-radicle-node-api/)
- [Radicle HTTP API (radicle-httpd) Issues Patches API](https://apis.io/collections/radicle/open-radicle-patches-api/)
- [Radicle HTTP API (radicle-httpd) Issues Repositories API](https://apis.io/collections/radicle/open-radicle-repositories-api/)
- [Radicle HTTP API (radicle-httpd) Issues Service API](https://apis.io/collections/radicle/open-radicle-service-api/)
- [Radicle HTTP API (radicle-httpd) Issues Source API](https://apis.io/collections/radicle/open-radicle-source-api/)
- [Radicle HTTP API (radicle-httpd) Issues Stats API](https://apis.io/collections/radicle/open-radicle-stats-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Radicle Httpd Overlay](https://apis.io/overlays/radicle/radicle-httpd-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Radicle Authentication](https://apis.io/security/radicle/radicle-authentication/)
- [Radicle Domain Security](https://apis.io/security/radicle/radicle-domain-security/)
- [Radicle Vulnerability Disclosure](https://apis.io/security/radicle/radicle-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://radicle.dev/)
- [Documentation](https://radicle.dev/guides)
- [Getting started](https://radicle.dev/guides/quick-start/)
- [Support](https://radicle.zulipchat.com)
- [Blog](https://radicle.dev/#updates)
- [Security](https://radicle.dev/.well-known/security.txt)
- [Terms of service](https://radicle.dev/legal)
- [GitHub](https://github.com/radicle-dev)

## API Evangelist rating

**Kin Score 44.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 42.9 |
| Contract governance | 4.5 |
| Operational transparency | 28.9 |
| Developer ergonomics | 72.0 |
| Access clarity | 28.6 |

**Agent readiness 28.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 26.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/radicle/](https://apis.io/providers/radicle/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Radicle: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/radicle/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
