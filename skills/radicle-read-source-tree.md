---
name: Read Radicle source code
description: Read a repository's source tree, file blobs and README at a given revision over the radicle-httpd JSON API.
api: openapi/radicle-httpd-openapi.yml
operations: [getRepo, getTree, getBlob, getReadme, getCommit]
---

# Read Radicle source code

Read-only workflow to browse the code in a seeded Radicle repository. No authentication required.

## Steps

1. **Resolve the repository and default branch.** Call `getRepo` (`GET /repos/{rid}`) and read `payloads["xyz.radicle.project"].data.defaultBranch` and `meta.head` (the head commit sha).
2. **List a directory.** Call `getTree` (`GET /repos/{rid}/tree/{sha}/{path}`) with `sha` = a commit id or branch head and `path` = a directory path. An invalid sha/path returns `code: 400`.
3. **Read a file.** Call `getBlob` (`GET /repos/{rid}/blob/{sha}/{path}`); check `binary` before using `content`.
4. **Read the README.** Call `getReadme` (`GET /repos/{rid}/readme/{sha}`).
5. **Inspect a commit.** Call `getCommit` (`GET /repos/{rid}/commits/{sha}`) for author, summary, parents and diff.

## Rules

- Always pass a concrete `sha` (a commit id or resolved branch head from `getRepo`) — the tree/blob/readme routes require a valid revision or they return `code: 400`.
- Errors use the `{error, code}` envelope; `code` mirrors the HTTP status.
- See conventions/radicle-conventions.yml and data-model/radicle-data-model.yml.
