# Cursor — Detailed Profile

> By Anysphere · VS Code Fork IDE · Pro: $20/month

## Overview

Cursor is the most mature AI-native IDE — a fork of VS Code with deep multi-file editing, codebase-wide context, and agentic workflows built into the editor itself. It switched from a fixed "fast request" model to token-based credit billing in June 2025, which caused significant community backlash but ultimately better reflects true compute costs.

## Pricing

| Plan | Price | Credits Included |
|------|-------|-----------------|
| Hobby (Free) | $0 | 2,000 completions + 50 slow requests/mo |
| Pro | $20/mo | $20 credit pool |
| Pro+ | $60/mo | $70 credit pool (3× Pro) |
| Ultra | $200/mo | $400 credit pool (20× Pro) |
| Teams | $40/user/mo | $20/user credit pool + org features |
| Enterprise | Custom | Pooled usage + compliance features |

Annual discount: 20% off (Pro = $16/month).

## Usage Limits (Pro)

### Credit System
Cursor Pro includes a **$20 monthly credit pool** billed at actual API rates. This is not a flat request counter — costs vary based on the model and task complexity.

### What Costs Credits

| Usage Type | Credit Impact |
|------------|---------------|
| Tab completions | Free (zero credits) |
| Auto mode (Cursor picks model) | Minimal / effectively free |
| Claude Sonnet 4.6 (manual select) | ~$0.09 per complex request |
| GPT-4o (manual select) | ~$0.08 per complex request |
| Large codebase context | Higher (more input tokens) |

### Practical Request Estimates (Pro)

| Task Type | Estimated requests before overage |
|-----------|----------------------------------|
| Auto mode only | Effectively unlimited |
| Standard premium model requests | ~225/month |
| Heavy multi-file agent tasks | ~80–120/month |

### After Credits Exhaust
1. Switch to Auto mode (free, no credits needed) for the rest of the month
2. Enable pay-as-you-go overages at standard API rates (no markup)
3. Upgrade to Pro+ or Ultra

## Context Window

Cursor points at your entire codebase using its own context management system. There is no single published token limit — it uses intelligent chunking to stay within model limits while loading the most relevant files.

## What's Included at Pro

- All frontier models: Claude Sonnet 4.6, GPT-4o, Gemini Pro, and others
- Unlimited Tab completions (AI autocomplete)
- Auto mode (Cursor selects the best model automatically)
- Extended Agent limits
- Cloud Agents (background tasks while you work on something else)
- MCPs, skills, and hooks
- Maximum context windows (full codebase awareness)
- Access to all Cursor AI features

## Upgrade Path

| Plan | Best For |
|------|----------|
| Pro+ ($60) | Developers hitting Pro limits regularly; saves money vs. overages |
| Ultra ($200) | Full-time AI-native developers spending 4+ hrs/day in Cursor |
| Teams ($40/user) | 3+ developers needing centralized billing, shared rules, SSO |

## The June 2025 Pricing Controversy

Cursor moved from 500 "fast requests" per month to credit-based billing in June 2025. Some users saw costs jump dramatically overnight. Cursor issued a public apology on July 4, 2025, acknowledged poor communication, and offered refunds for unexpected charges during the three-week transition window.

The new model is economically sound — it ties cost to actual compute consumed — but requires understanding the credit system to avoid surprises.

## Practical Tips

- Stay in Auto mode for everyday work — it's effectively unlimited and uses the best available model for each task
- Switch to manual premium models only for complex multi-file refactors or architectural tasks that need it
- Monitor your credit dashboard to catch patterns early
- If you consistently spend $20–40/month in overages, Pro+ is cheaper

## Strengths

- Most mature ecosystem and strongest community
- Widest model selection (Claude, GPT, Gemini)
- Tab completions and Auto mode are genuinely unlimited
- Pay-as-you-go overages at API rates — no markup, no lock-in

## Weaknesses

- Credit-based billing requires active monitoring
- Complex tasks can burn credits quickly
- No published hard token limit per session
- Pricing controversy eroded trust for some users

---

*Last updated: March 2026*
