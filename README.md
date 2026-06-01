# Design

Route standards-first design work to the right focused guidance. Use for design critique, visual polish, UX flows, accessibility, content, information architecture, service design, precedent study, lightweight design language extraction, or static HTML/CSS prototypes.

## Skill

This repository packages one portable agent skill:

- `design` - Route standards-first design work to the right focused guidance. Use for design critique, visual polish, UX flows, accessibility, content, information architecture, service design, precedent study, lightweight design language extraction, or static HTML/CSS prototypes.

The canonical skill body lives at `skills/design/SKILL.md`. Keep behavior changes there; keep this README focused on installation and packaging.

## Install

Clone the repository, then run the installer:

```bash
git clone https://github.com/cbzehner/skill-design.git
cd skill-design
./install.sh all
```

Install targets:

- `./install.sh claude` -> `~/.claude/skills/design`
- `./install.sh codex` -> `~/.codex/skills/design`
- `./install.sh agents` -> `~/.agents/skills/design` for generic agent harnesses such as Pi/Hermes-style setups
- `./install.sh opencode` -> `~/.config/opencode/skills/design`
- `./install.sh all --copy` copies files instead of symlinking

Manual installation is just a symlink or copy from `skills/design` into your agent's skills directory.

## Compatibility

This repo uses the common `skills/<name>/SKILL.md` layout so agents that understand file-based skills can load it directly. Host-specific metadata is included where useful:

- Claude Code: `.claude-plugin/plugin.json` and direct `~/.claude/skills` install
- Codex CLI: `.codex-plugin/plugin.json` with `skills: "./skills/"` and direct `~/.codex/skills` install
- Other agents: direct install to the agent's skills directory; unsupported frontmatter fields can be ignored

Some skills mention optional host tools such as `Task`, `Agent`, `Skill`, MCP tools, or browser automation CLIs. On hosts that do not provide those tools, adapt to equivalent local capabilities and keep the same workflow intent.

## Public Safety

These repositories are public. Do not commit organization-specific instructions, private repository names, secrets, tokens, cookies, raw session logs, customer data, or machine-local paths. Use environment variables and generic paths in examples.

## Repository Layout

```text
.claude-plugin/plugin.json   # Claude plugin metadata
.codex-plugin/plugin.json    # Codex plugin metadata
install.sh                   # Symlink/copy installer for common agent skill dirs
skills/design/SKILL.md
README.md
LICENSE
```

## License

MIT
