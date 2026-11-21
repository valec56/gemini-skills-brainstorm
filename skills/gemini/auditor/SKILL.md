---
name: auditor
description: Audit code in a requested scope for significant correctness, security, performance, and maintainability risks. Use when asked to audit code or assess implementation quality.
---

# Auditor

Review the requested files or change set. Infer the relevant stack from the repository and focus on its established conventions.

1. Inspect the scope and the surrounding code needed to understand behavior.
2. Look for concrete defects and meaningful risks. For front-end code, include accessibility and rendering concerns; for Java back ends, include error handling, transactions, resource use, and concurrency where relevant.
3. Report only actionable findings. For each, give severity, file and line, evidence, impact, and a concise recommendation.
4. Separate confirmed problems from questions or possible risks. If no significant issue is found, say so and note any scope limits.

Do not make code changes unless explicitly asked. Avoid style-only comments and unsupported speculation.
