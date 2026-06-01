# Design

Route design work to the right critique or production guidance. It covers visual polish, UX flows, accessibility, content, information architecture, and static HTML/CSS prototypes.

## Use It For

- Reviewing a UI for clarity and fit
- Planning a product flow or content structure
- Building a small design prototype in the current project style

## Install

Clone the repo and run the installer:

```bash
git clone https://github.com/cbzehner/skill-design.git
cd skill-design
./install.sh all
```

Install targets:

- `./install.sh claude` installs to `~/.claude/skills/design`
- `./install.sh codex` installs to `~/.codex/skills/design`
- `./install.sh agents` installs to `~/.agents/skills/design`
- `./install.sh opencode` installs to `~/.config/opencode/skills/design`
- `./install.sh all --copy` copies files instead of symlinking

Manual install works too: symlink or copy `skills/design` into your agent's skills directory.

## Agent Support

This repo uses the plain `skills/design/SKILL.md` layout. Claude Code and Codex also get small plugin manifests at `.claude-plugin/plugin.json` and `.codex-plugin/plugin.json`.

Other agents can read the same `SKILL.md` file. If a host does not support a frontmatter field or tool name, ignore that field and follow the workflow text.

## Layout

```text
.claude-plugin/plugin.json
.codex-plugin/plugin.json
install.sh
skills/design/SKILL.md
README.md
LICENSE
```

## Public Notes

These repos are public. Keep private repo names, secrets, customer data, raw logs, cookies, and absolute filesystem paths out of examples.

## License

MIT
