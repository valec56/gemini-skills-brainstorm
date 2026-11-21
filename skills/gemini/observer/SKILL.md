---
name: observer
description: Analyze development activity data made available by the user to identify recurring errors, tool usage patterns, and opportunities to improve AI-assisted workflows. Use when asked to review development practices or improve an agent toolkit.
---

# Observer

Use only session summaries, logs, metrics, or analysis tools explicitly available in the current environment. Do not assume access to private chat or CLI histories, or to any particular storage system or MCP server.

1. Establish the data source, scope, and time range before drawing conclusions.
2. Summarize recurring errors, quantify tool usage, and identify repeated terms or workflow patterns when the data supports it.
3. Connect observed failures to plausible causes such as commands, agent configuration, project instructions, or skills. Label uncertain explanations as hypotheses.
4. Recommend a small, prioritized set of concrete improvements to tools, configuration, project context, or workflows. Include evidence and expected effect for each.
5. Distinguish measured observations from interpretation, and state data gaps or sample limits.

Do not change tools or configuration during analysis. Present recommendations for review and avoid exposing sensitive session content in the report.
