# Claude Code — Detailed Profile

> By Anthropic · Terminal CLI · Pro: $20/month

## Overview

Claude Code is Anthropic's terminal-based agentic coding tool. Unlike IDE-based tools, it runs entirely in your terminal as a CLI, giving it direct, unrestricted access to your codebase, shell, and file system. It is powered by the same models available on claude.ai — Sonnet 4.6 and Opus 4.6.

It is widely considered to have the strongest raw AI reasoning among all coding tools, particularly for complex refactors, architectural thinking, and multi-file analysis.

## Pricing

| Plan | Price | Usage Multiplier |
|------|-------|-----------------|
| Pro | $20/mo | Baseline |
| Max 5× | $100/mo | 5× Pro usage |
| Max 20× | $200/mo | 20× Pro usage |
| API (pay-as-you-go) | Per token | Sonnet: $3/$15 per MTok in/out |

Annual billing: $17/month for Pro.

## Usage Limits (Pro)

### Session Window
Claude Code uses a **5-hour rolling window** — not a fixed daily reset. The window begins with your first message and expires 5 hours later. A new 5-hour window begins with the next message after expiry.

### Weekly Cap
In addition to the session window, a **weekly active hours cap** applies:
- ~40–80 active Sonnet hours per week
- Fewer hours when using Opus (which consumes 3–5× faster)
- "Active hours" = time Claude is processing tokens, not idle time

### Peak Hour Effect
During peak hours (approximately 5–11 AM PT / 1–7 PM GMT on weekdays), Anthropic adjusts the session window so that 5 hours of usage may resolve in less than 5 real clock hours. Roughly 7% of Pro users are affected by this.

### Model Cost Ratio (Pro quota consumption)
| Model | Relative Cost |
|-------|--------------|
| Sonnet 4.6 | 1× (baseline) |
| Opus 4.6 | 3–5× faster |

## Context Window

**200K tokens** across all models and plans (500K on Enterprise).

For very long conversations, Claude automatically summarizes earlier messages to preserve working context — your full history is retained but compressed to stay within the window.

## What's Included at Pro

- Claude Sonnet 4.6 (default)
- Claude Opus 4.6 (heavy quota cost)
- Claude Code CLI (terminal)
- Web, mobile, and desktop app
- Projects (with RAG-based document retrieval)
- Extended thinking mode
- MCP (Model Context Protocol) server support
- Usage shared across all Claude surfaces

## Overage Options

- Purchase extra credits on-demand without upgrading plan
- Upgrade to Max 5× or Max 20× for higher included usage

## Practical Tips

- Start new conversations frequently — long threads consume exponentially more tokens per message (message 30 in a thread can cost 80× more than message 1)
- Use `/compact` in Claude Code to manage context costs
- Use `/model` to switch between Sonnet and Opus based on task complexity
- Schedule heavy jobs during off-peak hours (evenings and weekends) for better throughput
- Use Opus only for tasks genuinely requiring its extra capability

## Strengths

- Best-in-class reasoning quality (Opus 4.6)
- Largest publicly disclosed context window at this price point
- Strong data controls and privacy practices
- Shared usage pool across all Claude surfaces is convenient

## Weaknesses

- Terminal only — no native IDE; requires VS Code extension for GUI
- Heavy Opus use exhausts Pro weekly limits by midweek
- Usage limits are dynamic and opaque (no precise token counter)
- Peak hour throttling can surprise users

---

*Last updated: March 2026*
