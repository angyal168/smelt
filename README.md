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


<!-- forge-usage:v1 -->

## What it actually does

`/smelt` takes raw material — a paper, a blog post, a YouTube transcript, a docs page, a
voice dump — and returns only the parts that change what you would think or do. The
metaphor is literal: burn off the slag, keep the metal.

It sorts what it finds into four buckets, and anything that fits none of them is dropped:

1. **Insights relevant to active projects** — facts, frameworks or techniques that connect
   to something you are already building.
2. **System improvements** — tools, workflows, automation patterns, prompting techniques.
3. **Business intelligence** — pricing models, market signals, competitive moves.
4. **Transferable knowledge** — anything that changes how you think, regardless of project.

Each surviving insight is written as three lines: the insight in one plain sentence, why it
matters (which project or system it touches), and what to do with it — a concrete next
action, not "consider exploring."

## What it deliberately throws away

This is the part that makes it useful, and it is written into the command:
background you already know, generic advice that applies to everyone, filler and
self-promotion, and — the important one — **things that sound smart but are not actionable.**
A summariser keeps those, because they summarise well. A smelter drops them.

## Usage

```bash
mkdir -p ~/.claude/commands
cp smelt.md ~/.claude/commands/
```

```
/smelt
<paste the transcript, paper, or article here>
```

You get back a Smelt Report: source, relevance, and the extracted insights in the
insight / why / what-to-do form.

## When not to use it

- When you want a faithful summary. Smelting is lossy on purpose; most of the source is
  supposed to disappear.
- For reference material you will need to quote accurately later — keep the original.
- On something you have not read at all and cannot sanity-check. The output is only as
  honest as your ability to notice when an "insight" was invented.

## Requirements

Claude Code with a `~/.claude/commands/` directory. If a project tracker is readable in the
session, `/smelt` scans it first so the relevance calls are grounded in your actual work.

<!-- /forge-usage:v1 -->


<!-- forge-siblings:v1 -->

## More from the same author

Other free, open-source Claude Code tools in this family. Each one stands
alone -- none of them depend on this repo, or on each other.

- [dar](https://github.com/angyal168/dar) -- Lightweight audit trail for Claude Code -- Discovery, Artifact, Receipt
- [ralph](https://github.com/angyal168/ralph) -- Autonomous iteration loop for Claude Code -- define task, set condition, let it run
- [serious](https://github.com/angyal168/serious) -- Precision mode for Claude Code -- no hype, no ambiguity, only what's true
- [forge-prompt](https://github.com/angyal168/forge-prompt) -- Prompt coaching for Claude Code -- rates, sharpens, and rewrites your prompts into action-first form
- [council](https://github.com/angyal168/council) -- AI advisory board for Claude Code -- 6 executive perspectives debate any decision
- [rally](https://github.com/angyal168/rally) -- Multi-agent coordination for Claude Code -- keep parallel agents in sync through a shared bus file
- [logos-protocol](https://github.com/angyal168/logos-protocol) -- Forge an AI that knows you, remembers, and ascends. Open source, free, yours to imprint

<!-- /forge-siblings:v1 -->

## Part Of

This command is part of the [Logos Protocol](https://github.com/angyal168/logos-protocol) -- an open protocol for building an AI assistant that actually knows you.

## License

MIT

<!-- forge-related:v1 -->

## Related

This repo is one module. It handles turning raw sources into something you can act on; it does not compose itself into a working system -- that wiring is a separate job.

- **[The Forge Content Marketing Skill Stack for Claude Code](https://andrewhangyal.gumroad.com/l/rbvkx?utm_source=github&utm_medium=readme&utm_campaign=gh-smelt)** -- a paid pack of Claude Code commands from the same author ($49).
- [All tools, free and paid](https://tools.aingyal.com/?utm_source=github&utm_medium=readme&utm_campaign=smelt) -- the full index.

Listed so you can find them if they are useful to you. Nothing here is required to use this repo, which stays free.

<!-- /forge-related:v1 -->
