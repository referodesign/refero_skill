![Refero Design Skill](assets/banner.png)

# Refero Skill

**Design with data**

Instead of guessing from training data, your agent researches 150,000+ real screens and flows from Stripe, Linear, Notion, and Figma before designing. Built-in craft knowledge on typography, color, copywriting, and anti-slop rules is included free — live search requires [Refero Pro](#unlock-live-design-research).

## Install

Works with Claude Code, Cursor, Gemini CLI, Lovable, and any MCP-compatible agent.

```bash
npx skills add referodesign/refero_skill
```

Craft knowledge loads immediately. No account required.

<details>
<summary>Manual installation</summary>

```bash
git clone https://github.com/referodesign/refero_skill.git
cp refero_skill/SKILL.md ~/.claude/skills/refero-design.md
```

On Claude.ai, add the contents of `SKILL.md` to your project knowledge.

</details>

---

## What's in the skill

**Live design research** — search across 150,000+ screens and 6,000+ user flows from real products. Every screen includes metadata on components, typography, colors, and layout. Requires Refero Pro.

**Craft knowledge** — typography scales, color systems, spacing, motion, icons, copywriting patterns, and anti-slop rules. Loads automatically, no account needed.

**Methodology** — a complete workflow from discovery questions through research, analysis, and implementation, with quality gates and validation.

<details>
<summary>Files</summary>

`SKILL.md` — Research-First methodology: discovery questions, research strategies, analysis frameworks, quality gates.

Reference guides: `typography.md`, `color.md`, `motion.md`, `icons.md`, `craft-details.md`, `anti-ai-slop.md`, `copywriting.md`, `mcp-tools.md`, `example-workflow.md`

</details>

---

## Unlock live design research

Get Refero Pro at [refero.design/mcp](https://refero.design/mcp), then connect your tool:

<details>
<summary>Claude Code</summary>

```bash
claude mcp add --transport http refero https://api.refero.design/mcp --header "Authorization: Bearer <token>"
```

</details>

<details>
<summary>Cursor</summary>

Add to `.cursor/mcp.json`:
```json
{
  "mcpServers": {
    "refero": {
      "url": "https://api.refero.design/mcp",
      "headers": { "Authorization": "Bearer <token>" }
    }
  }
}
```

</details>

<details>
<summary>Gemini CLI</summary>

```bash
gemini mcp add --transport http refero https://api.refero.design/mcp --header "Authorization: Bearer <token>"
```

</details>

<details>
<summary>Lovable</summary>

Settings → Connectors → New MCP server → `https://api.refero.design/mcp` → Bearer token

</details>

<details>
<summary>Other tools</summary>

```
URL: https://api.refero.design/mcp
Auth: Bearer <token>
```

</details>

The first time you call Refero, a browser window opens to sign in. After that it's automatic.

## Contributing

To add a new skill, create a directory under `skills/` with a `SKILL.md` file following the [Agent Skills](https://agentskills.io/) format.

## License

MIT
