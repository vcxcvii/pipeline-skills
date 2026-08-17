---
name: customer-story-extractor
description: >
  Turn raw customer evidence (support threads, QBR notes, call transcripts,
  Slack messages, NPS comments) into approved, checkable proof: a named case
  study, quotable lines, and a proof block for the homepage. Use when the user
  says they have happy customers but no case studies, needs testimonials, or
  their site claims "trusted by leading companies" without naming any.
---

# Customer Story Extractor (B2B SaaS)

Buyers discount every claim they cannot check. This skill converts evidence you
already have into evidence a skeptic can verify.

## Setup

Ask the user to paste any of: a QBR deck summary, a support thread where
something went right, a call transcript, renewal notes, or an NPS comment with
the free-text field. Two sources is enough to start.

Then ask the one question that decides everything: has this customer agreed to
be named, and if not, who would ask them?

## Extract

### 1. Find the before

The state the customer was in, in their words, with a number if one exists.
Look for time spent, headcount, error rates, cycle length, or revenue leaking.
If there is no number anywhere in the source, say so and use the sharpest
verbatim description instead. Do not estimate one.

### 2. Find the change

What specifically changed, when, and who noticed. The strongest proof is a
change a third party observed: the CFO stopped asking, the support queue
emptied, the auditor passed it.

### 3. Find the after

The number again, measured the same way. If the before and after were measured
differently, say that plainly in the story. Buyers who catch a mismatched
comparison stop believing everything else on the page.

### 4. Pull the quotes

Three verbatim lines maximum. Keep the customer's grammar. Cleaned-up quotes
read like marketing wrote them, because marketing did.

### 5. Mark what needs approval

Every name, number, and quote gets a status: cleared, needs approval, or
cannot use. Nothing without "cleared" goes on a public page.

## Output

- **Case study draft**: situation, what changed, result, quote. Under 400 words.
- **Proof block**: one sentence with a name and a number, sized for above the
  fold on a homepage.
- **Quote bank**: three quotes with role and company, each marked with approval
  status.
- **The approval email**: a short, specific request the user can send to the
  customer, naming exactly what will be published and where.
- **Evidence gaps**: what is missing to make this checkable.

## Rules

- Never invent a customer, a company, a role, or a number. Ever.
- Never publish an unapproved name. An anonymous case study is weak but honest;
  an unapproved named one is a customer relationship problem.
- Prefer one named customer with a modest number over five unnamed superlatives.
- Round numbers honestly and state the measurement window.
- No em-dashes.

## Related skills

`sales-one-pager` consumes this proof. `landing-page-teardown` will tell you
where the proof block belongs. `positioning-canvas` decides which claim the
proof has to support.
