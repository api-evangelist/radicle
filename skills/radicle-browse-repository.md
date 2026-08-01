---
name: Browse a Radicle repository
description: Discover a seeded repository on a Radicle node and read its issues, patches and commit history over the radicle-httpd JSON API.
api: openapi/radicle-httpd-openapi.yml
operations: [listRepos, getRepo, listIssues, listPatches, listCommits, getRepoActivity]
---

# Browse a Radicle repository

Read-only workflow against a public Radicle seed node (e.g. `https://seed.radicle.xyz/api/v1`). No authentication is required for these GET endpoints.

## Steps

1. **Find repositories.** Call `listRepos` (`GET /repos`, supports `page`/`perPage`) to list what the node seeds. Each item carries its `rid`, the `xyz.radicle.project` payload (name, description, defaultBranch), `delegates[]` and `visibility`.
2. **Load one repository.** Take a `rid` (form `rad:<base58>`) and call `getRepo` (`GET /repos/{rid}`). A missing/unseeded rid returns the `{error, code}` envelope with `code: 404`.
3. **List issues.** Call `listIssues` (`GET /repos/{rid}/issues`, filter with `state=open|closed`, page with `page`/`perPage`).
4. **List patches.** Call `listPatches` (`GET /repos/{rid}/patches`, filter `state=open|draft|archived|merged`).
5. **Walk history.** Call `listCommits` (`GET /repos/{rid}/commits`) or `getRepoActivity` (`GET /repos/{rid}/activity`) for the activity timestamp stream.

## Rules

- Identifiers: repo = `rad:...` (RID), node = `z6Mk...` (NID), actor = `did:key:...` (DID).
- Pagination is `page` (0-indexed) + `perPage`; responses are bare JSON arrays with no total-count. Stop when a page returns fewer than `perPage` items.
- Errors are a custom `{ "error": string, "code": integer }` envelope (not RFC 9457). Treat `code` as the HTTP status.
- See conventions/radicle-conventions.yml and errors/radicle-problem-types.yml.
