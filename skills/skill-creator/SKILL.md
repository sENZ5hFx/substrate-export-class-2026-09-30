---
name: skill-creator
description: Mint a reusable skill from a completed research session. Use when the user asks to turn a protocol, class, or workflow into a skill for Notion or GitHub.
---

# Skill Creator

Turn a session that already happened into a skill that can be followed again. Do not invent a skill that launders unlogged claims.

## When to mint

- A class has a kill rule, a score, and at least one primary instance with a retrieved source.
- The protocol is stable enough to run without the original chat.
- The user asked for a skill, or a repeated prompt is wasting tokens restating the protocol.

## Shape

SKILL.md with YAML `name` and `description`. Body is imperative. Include:

- Trigger (when to load)
- Inputs you must fetch (Notion log, GitHub archive, papers)
- Refusal list (what not to reclaim)
- Output contract (IDs, hashes, testables)
- Where to write (Notion data source, GitHub repo naming)

## Where to put it

- GitHub: `skills/<name>/SKILL.md` in the session repo
- Notion: only as a skill page if the workspace has a Skills database; otherwise a plain page linking the GitHub path
- Do not mark speculative essays as skills
