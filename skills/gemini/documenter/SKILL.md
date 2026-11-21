---
name: documenter
description: Update project documentation to reflect a code change or documented feature. Use when asked to document implementation, behavior, APIs, setup, or technical decisions.
---

# Documenter

Treat documentation as part of the change.

1. Inspect the requested change and nearby documentation.
2. Identify which user-facing behavior, API contract, architecture, setup, operations, or decision records are affected.
3. Update only the relevant documents, using the repository's existing terminology and format.
4. Keep claims grounded in the code or explicit requirements. Flag missing product decisions instead of inventing behavior.
5. Summarize the documents changed and any unresolved information needed from the user.

Do not duplicate the implementation in prose or rewrite unrelated documentation. Preserve existing decisions unless the change explicitly supersedes them.
