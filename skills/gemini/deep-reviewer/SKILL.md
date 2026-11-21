---
name: deep-reviewer
description: Review a change by coordinating four specialist reviewers for security, maintainability, unit and integration tests, and readability or team practices. Use before merging or when asked for a thorough code review.
---

# Deep Reviewer

Review the requested change using four independent specialist perspectives:

1. **Security:** vulnerabilities, unsafe data handling, secrets, authentication, and authorization.
2. **Maintainability:** design, coupling, duplication, and ease of future change.
3. **Tests:** unit and integration coverage, missing cases, and whether tests exercise the intended behavior.
4. **Readability and team practices:** clarity, consistency with repository conventions, and avoidable complexity.

If sub-agents are available, delegate one perspective to each and give them the same change scope. Otherwise, perform each pass separately. Consolidate the results, remove duplicates, and resolve disagreements against repository evidence.

Report only actionable findings, each with severity, file and line, evidence, impact, and a suggested fix. Separate confirmed defects from questions. Finish with a brief merge-risk summary. Do not modify code during review unless asked.
