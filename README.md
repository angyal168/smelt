# /smelt -- Extract Actionable Insights from Any Resource

> Burn off the slag. Keep the pure metal.

Paste in any raw material -- a research paper, blog post, YouTube transcript, documentation page, voice dump -- and /smelt strips it down to what actually changes how you think or act.

## Install

```bash
mkdir -p ~/.claude/commands
cp smelt.md ~/.claude/commands/
```

Then paste content and type `/smelt` in any Claude Code session.

## What It Does

1. Reads the full resource
2. Identifies which projects/systems it's relevant to
3. Extracts ONLY actionable insights (skips filler, background, generic advice)
4. Grades the source: Pure Gold / Good Ore / Low Yield / Slag
5. Saves a structured report to vault-staging

## Output Format

Each insight gets: what it is, why it matters, and what to do with it. No fluff. Most 5000-word articles yield 3 insights. That's fine -- most material is slag.

## Part Of

This command is part of the [Logos Protocol](https://github.com/angyal168/logos-protocol) -- an open protocol for building an AI assistant that actually knows you.

## License

MIT
