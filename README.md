![Refero Design Skill](assets/banner.png)

# Refero Design Skill

**Design with data, not defaults.**

AI agents design from training data averages. Generic layouts, safe colors, patterns you've seen a thousand times. This skill gives your agent something it never had: access to real design research.

## Real-time design research

Before creating anything, your agent searches [Refero](https://refero.design): 150,000+ screens and 6,000+ user flows from Stripe, Linear, Notion, Figma, Vercel, and thousands of the best products ever built.

Not just screenshots. Every screen has rich metadata: components, patterns, typography, colors, layout structures. Your agent doesn't just see designs, it understands them. User flows are broken down step by step: what each screen does, what content it shows, how users move through the experience.

Semantic search that finds anything. Pricing page with annual toggle? Fintech onboarding? Dark mode dashboard? Cancellation flow that reduces churn? If the pattern exists, your agent will find it. Research that takes designers hours, done in seconds.

Without this data, AI agents guess. They produce "safe" designs that look like everything else. With Refero, your agent researches first, then designs with confidence.

---

**Also in this skill:**

**Craft knowledge.** Deep guides on typography, color, spacing, motion, and icons. Letter-spacing rules, color token systems, animation timing curves. The details that separate polished products from rough prototypes.

**Anti-slop rules.** Explicit guidance to avoid the generic AI look: no default indigo, no blob backgrounds, no hero-features-pricing-FAQ templates. What makes design feel human versus generated.

**Methodology.** A complete workflow from discovery questions through research, analysis, and implementation. Quality gates and side-by-side validation against real products.

## Install

```bash
npx skills add referodesign/refero_skill
```

Requires [Refero MCP](#setup-refero-mcp) to connect your agent to the design library.

---

<details id="setup-refero-mcp">
<summary>Setup Refero MCP</summary>

### 1. Get your token

[refero.design](https://refero.design)

### 2. Connect

**Claude Code:**
```bash
claude mcp add --transport http refero https://api.refero.design/v1/mcp --header "Authorization: <token>"
```

**Gemini CLI:**
```bash
gemini mcp add --transport http refero https://api.refero.design/v1/mcp --header "Authorization: <token>"
```

**Cursor** — add to `.cursor/mcp.json`:
```json
{
  "mcpServers": {
    "refero": {
      "url": "https://api.refero.design/v1/mcp",
      "headers": { "Authorization": "<token>" }
    }
  }
}
```

**Lovable:** Settings → Connectors → New MCP server → `https://api.refero.design/v1/mcp` → Bearer token

**Other tools:**
```
URL: https://api.refero.design/v1/mcp
Auth: Bearer <token>
```

</details>

<details>
<summary>Troubleshooting</summary>

```bash
npx skills add referodesign/refero_skill --agent cursor
```

Or clone:
```bash
git clone https://github.com/referodesign/refero_skill.git .cursor/skills/refero-design
```

</details>

<details>
<summary>What's inside</summary>

**SKILL.md** — Research-First methodology
- Discovery questions before designing
- Research strategies and query patterns  
- Analysis frameworks and steal lists
- Design craft summaries
- Quality gates and validation

**Reference guides:**
- `typography.md` — Scale, pairing, letter-spacing, line-height
- `color.md` — Palettes, tokens, dark mode, contrast
- `motion.md` — Timing, easing, micro-interactions
- `icons.md` — Sizing, optical corrections, libraries
- `craft-details.md` — Focus states, forms, accessibility
- `anti-ai-slop.md` — Avoiding the generic AI look
- `mcp-tools.md` — Refero API reference
- `example-workflow.md` — Complete design walkthrough

</details>

## License

MIT
