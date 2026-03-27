# OpenAI Codex — Detailed Profile

> By OpenAI · Included in ChatGPT Plus · $20/month

## Overview

OpenAI Codex is an autonomous coding agent built into ChatGPT. It is not a standalone product — it is bundled into existing ChatGPT subscriptions at no additional cost. Codex operates in isolated cloud sandboxes with network access disabled during execution, making it one of the more security-conscious tools in this comparison.

It supports both cloud-based delegation (assign a task and come back later) and local CLI usage.

## Pricing

| Plan | Price | Codex Access |
|------|-------|-------------|
| Free | $0 | Limited (temporary promotion) |
| Go | $8/mo | Limited (temporary promotion) |
| Plus | $20/mo | Full Codex access |
| Pro | $200/mo | 10× Plus limits |
| Business | $30/user/mo | Team features + data privacy |
| Enterprise | Custom | Full enterprise controls |

> There is no standalone Codex subscription. You must have a ChatGPT plan.

## Usage Limits (Plus — $20/month)

### Session Window
Codex uses a **5-hour rolling window** identical in structure to Claude Code's session system.

### Messages Per 5-Hour Window

| Model | Approx. messages per 5 hrs |
|-------|---------------------------|
| GPT-5.1-Codex-Mini (light) | ~150–168 |
| GPT-5.3-Codex (standard) | ~60 |
| GPT-5.4 (heavy/frontier) | ~33 |

Actual limits vary based on:
- Task complexity (simple function vs. full PR implementation)
- Amount of context loaded (small script vs. large monorepo)
- Whether running locally (CLI) or in the cloud (web agent)

### After Hitting Limits
- Switch to GPT-5.1-Codex-Mini to extend your window
- Purchase additional credits without upgrading plan
- Use the Codex API with your own API key for pay-per-token access

## Context Window

**256K tokens** — the largest published context window among the tools in this comparison.

## Available Models

| Model | Use Case |
|-------|----------|
| GPT-5.1-Codex-Mini | Fast, low-cost; great for simple tasks and extending session limits |
| GPT-5.3-Codex | Balanced capability and cost |
| GPT-5.4 | Highest capability; use for complex reasoning tasks |

> GPT-4o is not available in Codex. The Codex model family is separate from the standard ChatGPT models.

## What's Included at Plus

**Codex features:**
- Codex CLI (terminal, runs locally or in cloud)
- Codex IDE extension (VS Code, Cursor, Windsurf)
- Cloud agent delegation (async task execution)
- GitHub integration (PR reviews, issue resolution via `@Codex`)
- Slack integration for task delegation
- Isolated sandbox execution with network disabled during runs

**Standard ChatGPT Plus features (also included):**
- GPT-5.2 access
- Image generation (DALL-E, Sora)
- Voice mode
- Advanced data analysis
- Web browsing

This bundling makes Plus exceptional value compared to standalone coding tools.

## Security Model

Codex runs in **isolated cloud containers**:
- Network access is disabled during code execution
- Each task runs in a fresh, sandboxed environment
- Code changes are committed in the sandbox for your review before merging
- You can review terminal logs and test outputs as verifiable evidence of actions taken

This is in contrast to tools like Google Antigravity, where agents have live terminal and filesystem access by default.

## GitHub Integration

Codex can:
- Automatically review PRs when tagged `@Codex`
- Resolve issues autonomously with a PR
- Run in CI/CD pipelines
- Access worktrees for parallel task execution

## Practical Tips

- Use GPT-5.1-Codex-Mini for simple tasks — it costs far less and extends session limits significantly
- Minimize AGENTS.md size — large agent context files consume tokens on every request
- Limit MCP servers — each MCP adds context overhead per message
- Use cloud delegation for long-running tasks so you can work on other things in parallel
- Scope tasks precisely — Codex performs best with clear, bounded instructions

## Strengths

- Best value if already paying for ChatGPT Plus ($20 total, not $40)
- Largest context window (256K tokens)
- Strong security model (isolated sandbox, network disabled)
- Async cloud delegation (fire and forget tasks)
- Deep GitHub integration

## Weaknesses

- Requires a ChatGPT subscription — no standalone option
- No dedicated IDE; extension-based only (VS Code, Cursor, Windsurf)
- Newer tool — less community ecosystem than Cursor
- Heavy frontier model (GPT-5.4) usage hits limits quickly (~33 tasks/5 hrs)

---

*Last updated: March 2026*
