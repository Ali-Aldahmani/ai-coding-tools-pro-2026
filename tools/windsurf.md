# Windsurf — Detailed Profile

> By Codeium · VS Code Fork IDE · Pro: $20/month (as of March 2026)

## Overview

Windsurf is a VS Code fork built around Codeium's native agentic architecture, **Cascade**. Its key differentiator is the SWE-1 model family — purpose-built coding agents that understand codebase structure natively, rather than general-purpose models adapted for coding.

In March 2026, Windsurf overhauled its pricing: moving from a credit-based system to quota-based plans and raising the Pro price from $15 to $20/month. This eliminated its primary competitive advantage (price) over Cursor, making SWE-1 the sole remaining differentiator for most users.

## Pricing

| Plan | Price | Credits / Quota |
|------|-------|----------------|
| Free | $0 | 25 prompt credits/month |
| Pro | $20/mo | ~500 prompt credits/month |
| Max | $200/mo | Significantly larger quota |
| Teams | Varies | 500 credits/user/month + pooled add-ons |
| Enterprise | Custom | 2× Teams quota + RBAC + SSO |

> Early Adopter pricing is locked through end of 2026 for existing Pro and Teams subscribers. New subscribers from March 2026 onward pay the new prices.

Annual billing: available with discount.

## Usage Limits (Pro)

### Monthly Prompt Credits
Pro includes approximately **500 prompt credits per month**:
- Credits reset on your billing date — **no rollover**
- 500 credits ≈ 500 messages at standard model rates (one credit per prompt)
- At 16–17 prompts per day, Pro covers most individual developer workflows

### Credit Cost by Model

| Model | Credits per prompt |
|-------|--------------------|
| SWE-1 | 1 cr |
| SWE-1.5 | 1 cr |
| SWE-1-mini | 1 cr |
| GPT-5.1-Codex (0 cr tier) | 0 cr |
| GPT-5.2 (standard) | 1 cr |
| GPT-5.3 (enhanced) | 2–3 cr |
| Claude Sonnet 4.6 | 2 cr |
| Gemini 3.1 Pro | 2 cr |
| Large context variants (1M token) | 2.5–4× standard rate |
| Fast mode (priority queue) | 2× standard rate |

### What Is Always Free

| Feature | Cost |
|---------|------|
| Tab completions (inline autocomplete) | Always free |
| Inline edits | Always free |
| File creation, editing, search (tool calls) | Free (don't count toward credits) |
| Failed operations | Free (no credit deducted) |

> This is Windsurf's key billing feature: **you pay only for the initial prompt, not for the internal actions Cascade takes to fulfill it** — whether it searches 50 files, creates 10 new ones, or runs the test suite.

### Add-On Credits
When monthly credits run out:
- Add-on credits: **$10 for 250 credits** (individual) / **$40 for 1,000 pooled credits** (teams)
- Add-on credits **do roll over** and never expire (require active subscription to use)
- Auto-refill: triggers when balance drops below 15 credits; configurable cap ($160/month default maximum)

## Context Window

Windsurf uses standard context windows for most models. Large context variants (up to 1M tokens) are available but cost 2.5–4× the standard credit rate.

## Native Models: SWE-1 Family

The SWE-1 models are Windsurf's native coding agents — built specifically for software engineering tasks, not adapted from general-purpose LLMs.

| Model | Best For |
|-------|----------|
| SWE-1 | Complex architectural tasks; full codebase understanding |
| SWE-1.5 | Fast iteration; rapid feature implementation |
| SWE-1-mini | Quick edits, small scripts, quota-conscious use |

All three SWE models are charged at 1 credit per prompt regardless of internal complexity.

## Cascade: How the Agent Works

Cascade is Windsurf's agent architecture:
- You send one message — Cascade handles planning, file navigation, editing, testing
- Every internal action (file search, code write, test run) is free
- Only your initial prompt costs a credit
- If Cascade fails mid-task (e.g., file not found), no credit is charged

This "you pay for the ask, not the work" model makes Windsurf billing more predictable than token-based tools.

## What's Included at Pro

- SWE-1, SWE-1.5, SWE-1-mini (native agents)
- All third-party frontier models (Claude, GPT, Gemini)
- Unlimited Tab completions
- Cascade agent with full codebase access
- Windsurf Previews (live app preview in IDE)
- Fast Context (retrieval across large codebases)
- Auto-refill credits option
- Student discount: 50% off with `.edu` email

## Practical Tips

- Use SWE-1-mini for routine tasks to conserve credits
- Use GPT-5.1-Codex (0 cr) for simple autocomplete-style tasks — it's literally free
- Avoid Fast mode unless you're in a time crunch — it doubles the credit cost
- Avoid large context variants unless you actually need to process the full 1M token window
- Use Continue wisely — each "continue" is a new prompt and costs a credit
- Track your usage in the dashboard; enable auto-refill to avoid interruptions on critical work

## Strengths

- Most predictable billing model (1 prompt = 1 credit; tool calls are free)
- Native SWE-1 models designed specifically for coding
- Cascade's "pay for ask, not for work" pricing is fair for complex agentic tasks
- Tab completions and inline edits always free
- Add-on credits roll over (don't lose what you paid for)
- 50% student discount

## Weaknesses

- Lost price advantage vs. Cursor ($15 → $20 in March 2026)
- 500 credits thin for heavy users — typical power user needs 1,000–2,000/month
- Monthly credits don't roll over — lose them if you don't use them
- SWE-1 quality vs. Claude Opus / GPT-5.4 on complex reasoning tasks is debated
- No browser agent (unlike Antigravity)

---

*Last updated: March 2026*
