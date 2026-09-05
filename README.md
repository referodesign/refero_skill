![Refero Design Skill](assets/banner.png)

# Refero

Refero packages one design skill and one read-only MCP connection for AI design work.
The skill makes research mandatory before implementation. With live Refero research, agents
can use curated visual styles, 150,000+ real app screens, and 6,000+ user flows from
well-designed products.

## Install

### ChatGPT / Codex

[Install Refero from the OpenAI Plugins Directory](https://chatgpt.com/plugins/plugin_asdk_app_6a72258e6f18819183e5c4d8a56b78d9).

The plugin includes Refero MCP and Refero Skill. Sign in with your Refero account when prompted; no manual MCP config or separate skill installation is needed. Live research requires a paid Refero plan. See the [setup guide](https://doc.refero.design/mcp/getting-started).

### Codex app and CLI — install from GitHub

```bash
codex plugin marketplace add referodesign/refero_skill
codex plugin add refero@refero
```

Restart the app after installation. The first connection opens Refero in the browser for
OAuth sign-in.

### Claude Code

```text
/plugin marketplace add referodesign/refero_skill
/plugin install refero@refero
```

### Gemini CLI

```bash
gemini extensions install https://github.com/referodesign/refero_skill
```

### Cursor

After the marketplace listing is approved, open Cursor's plugin marketplace or run
`/add-plugin` and search for **Refero**.

### Standalone skill

Use this when the client already has Refero MCP configured or only the design methodology
is needed:

```bash
npx skills add https://github.com/referodesign/refero_skill --skill refero-design
```

No account is required for the bundled craft references. Live Refero research uses OAuth
when the MCP client first connects to `https://api.refero.design/mcp`.

## What it does

1. Researches visual styles first, then real screens and user flows when the task needs them.
2. Extracts concrete patterns and locks references before implementation.
3. Applies bundled guidance for typography, color, spacing, motion, icons, and copywriting.
4. Keeps design decisions tied to evidence instead of generic AI defaults.
5. Checks substantial visual work against the selected direction before handoff.

## What is included

- `skills/refero-design/` — the single canonical skill and its references.
- `.mcp.json` — Refero MCP for Codex and Claude Code plugin installs.
- `mcp.json` — Refero MCP for Cursor plugin installs.
- `gemini-extension.json` — Gemini CLI extension manifest.
- `.codex-plugin/`, `.claude-plugin/`, and `.cursor-plugin/` — platform metadata.
- `server.json` — official MCP Registry metadata.

All connection manifests use the same production endpoint and contain no access tokens.

## Existing standalone installations

Older clones placed `SKILL.md` at the repository root. Remove that old installation and
run the standalone install command again. The current skill lives at
`skills/refero-design/SKILL.md`; keeping both layouts creates duplicate skills.

For manual installation, copy the entire `skills/refero-design/` directory into the
client's skills directory so its `references/` files remain beside `SKILL.md`.

## Validate a release

```bash
scripts/check-release
```

The check validates manifests, versions, local links, the canonical MCP URL, package
boundaries, and common secret leaks. Platform-native validation and clean-profile install
tests are still run before tagging a release.

## Security

Report vulnerabilities privately to [support@refero.design](mailto:support@refero.design).
See [SECURITY.md](SECURITY.md) for details.

## License

MIT
