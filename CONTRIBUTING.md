# Contributing

Pull requests are welcome, including from people who have never opened a PR
before. If the process is the blocker, open an issue with the skill text and we
will handle the mechanics.

## The bar a skill has to clear

1. **One job.** A skill does one thing a specialist would recognise as a task.
   "Fix marketing" is not a skill.
2. **A named lever.** State which of reach, capture, convert, or compound it
   moves. If it does not move one, it does not belong here.
3. **A real setup step.** What does the agent need from the user before it can
   start? Ask for the minimum, and say what to do when the user cannot provide
   it.
4. **A pasteable artifact.** The output is a page, a sequence, a spec, a
   document. Not a list of considerations.
5. **Explicit refusals.** Every skill states what it must never invent, and what
   it should tell the user honestly even when the news is bad.
6. **Related skills.** Point at the neighbouring skills so the set behaves like
   a system.

## Format

```
skills/<skill-name>/SKILL.md
```

Frontmatter:

```yaml
---
name: skill-name
description: >
  What it does, then "Use when..." describing the user's situation in the
  user's own words. This is what an agent matches against, so write triggers,
  not marketing.
---
```

## House style

- No em-dashes.
- No AI-slop vocabulary: leverage, unlock, elevate, seamless, robust, empower,
  game-changing, in today's fast-paced.
- Figures, not magnitude words: `$100K+`, never "six figures".
- One idea per sentence. If it needs a semicolon, it is two sentences.
- British or American spelling both fine, just be consistent inside a file.

## Testing a skill before you submit

Run it three times on real inputs, including one where the input is
deliberately thin. A skill that produces confident output from missing evidence
is the failure mode we care most about catching.

Then check: did it invent anything? A name, a number, a quote, a certification?
If yes, the refusal section needs to be stronger.
