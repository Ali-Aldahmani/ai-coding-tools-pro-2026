# Google Antigravity — Detailed Profile

> By Google · Agent-First IDE · Free (preview) / $20/month via Google AI Pro

## Overview

Google Antigravity is an agent-first IDE launched in public preview on November 18, 2025. Built on a VS Code fork, it is designed from the ground up for task-level, autonomous development — rather than bolting AI onto a traditional code editor. Agents have direct, simultaneous access to your editor, terminal, and browser.

During its preview phase, Antigravity offers free access to Claude Opus 4.6 (Thinking) — a model that costs $100–200/month through other tools. This makes it the highest raw AI value available at zero cost, with the significant caveat that rate limit instability has caused real workflow disruptions in early 2026.

## Pricing

| Plan | Price | Notes |
|------|-------|-------|
| Individual (preview) | $0 | Public preview; quotas unpublished |
| Google AI Pro | $20/mo | Higher rate limits; AI credits included |
| Google AI Ultra | $249.99/mo | Highest limits; all Google AI features |
| Add-on credits | $25 / 2,500 credits | Can be purchased on any paid plan |

> Existing subscribers keep legacy pricing. New subscribers from March 2026 onward use the new credit/quota system.

## Usage Limits

### Preview (Free Individual)
- Quota-based with 5-hour refresh cycles
- Exact limits are not published by Google
- Originally described as "high" and "generous" — significantly reduced in March 2026
- Full feature access (no model gating)

### Google AI Pro ($20/month)
- Higher rate limits than free tier
- AI credits shared across the Google AI ecosystem (Antigravity, Gemini CLI, NotebookLM, etc.)
- Additional credits: $25 for 2,500

### Credit Top-Up
| Credit Pack | Cost |
|------------|------|
| 2,500 credits | $25 |

Note: Google has not published exactly what one credit buys within Antigravity specifically.

### Rate Limit Crisis (March 2026)
On March 11, 2026, Google introduced a credit system and reduced quotas significantly, citing "incredible demand that exceeded expectations." This change resulted in:
- Pro subscribers experiencing 7-day lockouts
- Community complaints about "Unacceptable Antigravity Quotas" blocking workflows
- Google's AI for Developers forum overwhelmed with reports

## Available Models

All models are available on all plans — no model gating between free and paid tiers.

| Model | Notes |
|-------|-------|
| Gemini 3.1 Pro (High) | Google's flagship; high capability |
| Gemini 3.1 Pro (Low) | Faster, more quota-efficient |
| Gemini 3 Flash | Fastest response; lowest quota cost |
| Claude Opus 4.6 (Thinking) | Best reasoning; normally $100–200/mo elsewhere |
| Claude Sonnet 4.6 | Balanced performance |
| GPT-OSS 120B | Open-source large model |

## Interface: Editor View + Agent View

Antigravity introduces two distinct interaction modes:

**Editor View** — traditional AI-powered IDE:
- Tab completions (unlimited on all plans)
- Inline commands
- Chat assistant in sidebar

**Agent View** — autonomous task execution:
- Agents plan, execute, and verify tasks without constant human input
- Direct access to: editor, terminal, browser
- Agent Skills: save reusable context and workflows to a knowledge base
- Agent Manager: spawn and monitor multiple agents simultaneously
- Parallel multi-agent sessions (added in Wave 13)

## Unique Features

- **Browser subagent:** Agents can launch Chrome, interact with UI, test user flows, and verify functionality — no other Pro-tier tool offers this natively
- **Agent Skills:** Save useful context and code patterns so agents improve over future tasks
- **Artifacts:** Agents communicate progress via screenshots and walkthroughs
- **Plan Mode:** Smarter task planning before execution (Wave 13)
- **Arena Mode:** Blind model comparison to help choose the best model for your workflow

## Security Concerns ⚠️

Antigravity agents have **autonomous access** to:
- Your terminal (can run any shell command)
- Your filesystem (can read and write any file)
- Your network (live internet access during execution)

Known issues as of March 2026:
- 5 additional vulnerabilities documented by researcher Johann Rehberger (late 2025)
- Widely-cited incident: one user's entire D drive wiped by an agent
- macOS sandbox added February 23, 2026 — restricts terminal commands to workspace
- **Windows and Linux users have no sandbox protection yet**

Recommended mitigations:
- Use Review-driven development mode (agent asks permission before each action)
- Avoid running on repositories containing secrets, credentials, or sensitive data
- Keep a backup/snapshot of important directories

## Setup

1. Download from `antigravity.google/download` (~300–400 MB)
2. Run installer on macOS, Windows, or Linux
3. Import settings from VS Code or Cursor (optional)
4. Choose agent mode: Autopilot / Auto / Manual (Off)
5. Sign in with Google account; subscription status syncs automatically

## Practical Tips

- Use Gemini 3 Flash or GPT-OSS for simple tasks to conserve quota
- Reserve Claude Opus 4.6 (Thinking) for genuinely complex architectural tasks
- Always keep a backup tool (Cursor or Claude Code) ready for when quotas run out
- Enable Review mode for production codebases — don't trust Autopilot on critical files
- Monitor quota usage closely; 7-day lockouts are not theoretical

## Strengths

- Free Claude Opus 4.6 (Thinking) — the most powerful coding model available at any price
- Built-in browser agent for end-to-end UI testing
- Full feature parity across all tiers (no model gating)
- Agent Skills for persistent, improving workflows
- Multi-model access in a single IDE

## Weaknesses

- Rate limit crisis ongoing — Pro subscribers hitting 7-day lockouts (March 2026)
- No sandbox protection on Windows/Linux
- Quota limits opaque and subject to sudden reduction
- Community trust significantly damaged by March 2026 changes
- Newer and less stable than Cursor or Claude Code

---

*Last updated: March 2026*
