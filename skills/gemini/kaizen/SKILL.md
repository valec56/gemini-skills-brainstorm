---
name: kaizen
description: Analyze Gemini CLI session metrics exposed by the Kaizen MCP server to find recurring errors, tool usage patterns, and configuration or workflow improvements. Use when asked to review Gemini CLI usage or improve the development setup.
---

# Kaizen

Use the Kaizen MCP server as the source of session data. It is a TypeScript stdio MCP server that reads Gemini CLI sessions recorded in Basic Memory's SQLite database. Do not assume direct database access when MCP tools are unavailable.

1. Inspect the available session data and its time range before drawing conclusions.
2. Summarize error logs, quantify tool usage, and identify recurring keywords or patterns. Include counts or proportions when the data supports them.
3. Connect observed failures to likely causes, such as a command, Gemini CLI setting, project instruction, or skill. Mark uncertain causes as hypotheses.
4. Recommend a small, prioritized set of concrete improvements to tools, Gemini CLI configuration, project context, or workflows. Include evidence and expected effect for each.
5. Distinguish measured observations from interpretation, and state data gaps or sample limits.

Do not change configuration or tools during analysis. Present proposed changes for review; avoid exposing sensitive session content in the report.
