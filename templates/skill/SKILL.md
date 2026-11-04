---
name: skill-name
description: "What this skill does and when to use it, in one or two sentences. Agents read this line to decide whether to load the skill, so name the tasks and outputs."
---

# Skill name

One paragraph: what the job is, what a good result looks like, and what the skill does not do.

## Load first

- Files or notes the agent must read before starting.
- `FEEDBACK.md` in this folder: past corrections.

## Steps

1. …
2. …

## Rules

- Each rule comes from a real correction. Keep the why next to it.

## Check before sending

- How to verify the output before handing it over.

## Guardrails

- What the agent must never do without asking.

## Feedback log

After each run, add an entry to `FEEDBACK.md`. When the same correction shows up twice, or you state it as a rule, move it into this file and mark the entry as promoted.
