# hegel-skill

An [Agent Skill](https://agentskills.io) that teaches agents how to write property-based tests using [Hegel](https://github.com/hegeldev/hegel-core). 

When you ask an agent to write property-based tests, this skill provides:

- A methodology for identifying testable properties from code evidence
- Generator discipline guidelines to avoid over-constraining inputs
- Language-specific API references and idiomatic patterns
- Guidance on evolving existing unit tests into property-based tests

This currently only supports [hegel-rust](https://github.com/hegeldev/hegel-rust) but we will update it for each language's Hegel library as new ones come out.

## Installation

This should work with Claude Code, Codex, and any agent that supports the Agent Skills standard.

### Claude Code

Add the marketplace and install:

```bash
/plugin marketplace add hegeldev/hegel-skill
/plugin install hegel-skill@hegeldev-hegel-skill
```

Or for local development:

```bash
claude --plugin-dir path/to/hegel-skill
```

### Codex

Use the built-in skill installer:

```
$skill-installer install https://github.com/hegeldev/hegel-skill/tree/main/skills/hegel
```

Or copy the skill directory manually:

```bash
cp -r skills/hegel ~/.codex/skills/hegel
```

### Any Agent (cross-client)

Copy the skill into your project's `.agents/skills/` directory:

```bash
cp -r skills/hegel .agents/skills/hegel
```

Or use npx:

```bash
npx skills add hegeldev/hegel-skill
```
