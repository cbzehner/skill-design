# Design Skill

Compact router for standards-first web design workflows.

This repository replaces the direct trigger surface of `skill-boring-web-design` with one canonical `design` skill. The original guidance is preserved under `skills/design/references/` and loaded only when relevant.

## Modes

- `critique` - design review and prioritized fixes
- `visual` - layout, typography, color, spacing, hierarchy, polish
- `ux-flow` - flows, forms, states, onboarding, recovery
- `accessibility` - semantic HTML, keyboard behavior, focus, contrast, ARIA
- `content` - product copy, labels, CTAs, errors, empty states
- `information-architecture` - navigation, labels, taxonomy, page hierarchy
- `service` - journeys, touchpoints, operations, trust, failure recovery
- `precedent` - reference study and taste-building without copying
- `language` - lightweight design language extraction
- `static-html` - self-contained static prototypes

## Installation

Symlink the skill:

```bash
ln -sfn ~/Developer/Personal/skill-design/skills/design ~/.claude/skills/design
ln -sfn ~/Developer/Personal/skill-design/skills/design ~/.codex/skills/design
```

Restart the agent session after installing so the skill list is reloaded.

## License

MIT
