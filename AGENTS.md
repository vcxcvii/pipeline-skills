# Working with these skills

Guidance for any agent running a skill from this repository.

## The four levers

Every skill serves exactly one lever of a pipeline. When a user describes a
problem, place it before choosing a skill.

| Lever | The question it answers | Skills |
| --- | --- | --- |
| Reach | Do the right people find us? | `aeo-page-audit`, `founder-content-engine`, `campaign-brief-builder` |
| Capture | Do they turn into conversations? | `landing-page-teardown`, `outbound-sequence-writer` |
| Convert | Do conversations turn into revenue? | `positioning-canvas`, `icp-sharpener-b2b`, `sales-one-pager`, `customer-story-extractor` |
| Compound | Do we know what worked and repeat it? | `gtm-dashboard-spec` |

If more than one lever is broken, run `positioning-canvas` first. Everything
downstream inherits the claim it produces, so fixing pages or sequences before
the claim is settled means rewriting them twice.

## Rules that apply to every skill

1. **Never fabricate evidence.** No invented customers, quotes, statistics,
   logos, case studies, or certifications. When evidence is missing, say it is
   missing and mark the claim unproven. This rule outranks producing a
   complete-looking deliverable.
2. **Ask for the minimum input, then start.** Two real inputs beat a
   questionnaire. Ask for what changes the output, not for what is nice to know.
3. **Produce artifacts, not advice.** The output should be pasteable: a page, a
   sequence, a one-pager, a spec. "Consider testing different headlines" is not
   an output.
4. **Stop before anything sends.** Outbound and publishing skills end at a human
   approval step. Never send, post, or publish.
5. **Say when the answer is no.** If the product is not differentiated, if the
   channel is wrong, if the data does not support the claim, say so plainly.
6. **House style**: no em-dashes, no "leverage", "unlock", "seamless",
   "robust", "game-changing". Write figures as `$100K+`, never "six figures".
   One idea per sentence.

## Output conventions

- Markdown, ready to paste.
- Lead with the answer, then the reasoning. Never build suspense.
- Score things against a stated rubric when you score them, and show the rubric.
- End with what is missing: the evidence gaps the user has to fill.

## Repository conventions

- One skill per directory under `skills/`, containing a single `SKILL.md`.
- Frontmatter needs `name` and a `description` written so an agent can tell,
  from the description alone, when to trigger it. Describe the user's situation
  in the user's words.
- Every skill ends with a **Related skills** section pointing at its neighbours.
