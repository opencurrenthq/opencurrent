# OpenCurrent plugin

에이전트에 바로 연결하는 최신 AI 활용법. One install connects your coding agent to [OpenCurrent](https://opencurrent.ai) and adds one skill, `latest-first`: before an agent-setup task (MCP, skills, hooks, subagents, plugins, CI), the agent looks up the latest dated method and follows it.

## Install

Claude Code

```
claude plugin marketplace add opencurrenthq/opencurrent
claude plugin install opencurrent@opencurrent
```

Codex

```
codex plugin marketplace add opencurrenthq/opencurrent
codex plugin add opencurrent@opencurrent
```

No key needed (200 full workflows per day per IP). A free key from https://opencurrent.ai/account/keys raises the limit.

## What it sends

Search words and workflow ids to https://opencurrent.ai/mcp. Never your code, files or conversation. The server is read-only.

## What is inside

- `.mcp.json` / `mcp.json`: the remote MCP server https://opencurrent.ai/mcp
- `skills/latest-first/SKILL.md`: when to look things up and how to follow them
