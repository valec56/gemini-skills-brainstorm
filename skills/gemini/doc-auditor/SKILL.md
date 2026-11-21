---
name: doc-auditor
description: Check whether project documentation matches the implemented behavior, API contracts, and project decisions. Use for documentation audits or consistency checks.
---

# Doc Auditor

Perform an independent, read-only comparison of documentation and implementation.

1. Inspect the requested documents and the relevant code or API definitions.
2. Check for contradictions, outdated instructions, undocumented behavior, and claims unsupported by the implementation.
3. Report each discrepancy with document location, code location, evidence, and practical impact.
4. Distinguish confirmed mismatches from ambiguous requirements. Rank findings by user or operational impact.
5. State which areas you could not verify and why.

Do not edit documentation or code during the audit. Do not treat missing documentation as a defect when the behavior is out of scope or not established.
