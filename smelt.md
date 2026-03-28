Smelt -- strip a resource down to what you can actually use.

Paste in raw material: a science paper, blog post, YouTube transcript, documentation page, voice dump, or anything else. Your job is to burn off the slag and extract pure usable metal.

## What you're looking for

1. **Insights relevant to active projects** -- facts, frameworks, techniques, or references that connect to something in the project tracker. If you can read the tracker, scan it first.

2. **System improvements** -- better tools, workflows, automation patterns, prompting techniques, or infrastructure ideas that would improve how the workspace operates.

3. **Business intelligence** -- market signals, pricing models, competitive moves, technology shifts, revenue opportunities.

4. **Transferable knowledge** -- anything that changes how we think or act, regardless of which project it touches.

## How to smelt

1. Read the pasted resource completely
2. Identify which project(s) or system(s) it's relevant to
3. Extract ONLY what changes how we think or act. Skip:
   - Background info already known
   - Generic advice that applies to everyone
   - Filler, introductions, self-promotion
   - Things that sound smart but aren't actionable
4. For each extracted insight, write:
   - **The insight** (one sentence, plain language)
   - **Why it matters** (connects to which project/system)
   - **What to do with it** (concrete next action or integration point)

## Output format

```
# Smelt Report -- [Source Title or Description]
> Source: [URL or description]
> Smelted: [date]
> Relevance: [project names]

## Pure Metal (high-value extractions)

### 1. [Insight title]
[The insight in one sentence]

**Relevance**: [project/system]
**Action**: [what to do with this]

### 2. [Next insight]
...

## Slag (noted but not actionable now)
- [thing noticed but can't use yet]
- [thing that might matter later]

## Verdict
[One sentence: was this resource worth the smelt? Grade: Pure Gold / Good Ore / Low Yield / Slag]
```

## Where it goes

- Save the smelt report to `vault-staging/smelted/YYYY-MM-DD_HHMM_[slug].md`
- If any insight is immediately actionable, flag it: "This one's hot -- want me to act on [specific thing] now?"

## Rules

- Be ruthless. A 5000-word article might yield 3 insights. That's fine. Most material is slag.
- Write in the user's voice, not academic voice. "This changes how we think about X" not "This finding has implications for..."
- If the resource is garbage, say so. "Low yield. Nothing here we don't already know." Don't stretch to find value.
- If something is pasted without context, ask ONE question: "What were you thinking when you saved this?" Then smelt based on the answer.
