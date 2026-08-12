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

<!-- forge-related:v1 -->

## Related

This repo is one module. It handles turning raw sources into something you can act on; it does not compose itself into a working system -- that wiring is a separate job.

- **[The Forge Content Marketing Skill Stack for Claude Code](https://andrewhangyal.gumroad.com/l/rbvkx?utm_source=github&utm_medium=readme&utm_campaign=smelt)** -- a paid pack of Claude Code commands from the same author ($49).
- [All tools, free and paid](https://tools.aingyal.com/?utm_source=github&utm_medium=readme&utm_campaign=smelt) -- the full index.

Listed so you can find them if they are useful to you. Nothing here is required to use this repo, which stays free.

<!-- /forge-related:v1 -->
