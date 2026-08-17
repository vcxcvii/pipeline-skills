# Pipeline Skills

Free GTM skills for AI agents, built for founder-led B2B SaaS teams.

These are the workflows we actually run on client work at [Grow &
Close](https://growandclose.com?ref=pipeline-skills): positioning, landing
pages, outbound, AI-search visibility, sales enablement, customer proof, and
GTM measurement. They work in Claude Code, Claude Desktop, and any agent that
reads the [Agent Skills](https://agentskills.io) format.

Ten skills. No signup, no email gate, MIT licensed.

## What is a "skill", in plain language

A skill is a markdown file that teaches an AI agent how to do one job properly:
what to ask you for, what steps to follow, what good output looks like, and what
it must never make up. Without one, you get a generic answer. With one, you get
the same process a specialist would run.

You do not need to code. If you can copy one line into a terminal, you can use
these.

## Install

In Claude Code:

```
/plugin marketplace add vcxcvii/pipeline-skills
```

Then restart Claude Code. That is it. Ask for what you want in plain English
and the right skill picks itself up:

> "Tear down our homepage: https://example.com"

> "Our sequences get no replies, help me rebuild one"

> "Turn these QBR notes into a case study"

Prefer to install manually? Copy any folder from `skills/` into your project's
`.claude/skills/` directory, or into `~/.claude/skills/` to have it everywhere.

## The skills, organised by what is broken

We group everything by the four levers of a pipeline. Start with the one that is
actually stuck, not the one that sounds most interesting.

### Reach: the right people are not finding you

| Skill | Use it when |
| --- | --- |
| [aeo-page-audit](skills/aeo-page-audit/) | AI answers recommend competitors instead of you, and you want to know why |
| [founder-content-engine](skills/founder-content-engine/) | Your founder posts inconsistently, or the content sounds like everyone else's |
| [campaign-brief-builder](skills/campaign-brief-builder/) | You have a calendar of activities but no single argument connecting them |

### Capture: they find you and do not convert

| Skill | Use it when |
| --- | --- |
| [landing-page-teardown](skills/landing-page-teardown/) | Traffic arrives and nothing happens, and you need a scored critique with rewrites |
| [outbound-sequence-writer](skills/outbound-sequence-writer/) | Your sequences read like every other AI-written email and get no replies |

### Convert: conversations do not become revenue

| Skill | Use it when |
| --- | --- |
| [positioning-canvas](skills/positioning-canvas/) | Buyers cannot tell you apart, and every team tells a different story |
| [icp-sharpener-b2b](skills/icp-sharpener-b2b/) | "We sell to B2B companies" is still your best answer on who to target |
| [sales-one-pager](skills/sales-one-pager/) | Deals stall after a good demo and your champion cannot sell it internally |
| [customer-story-extractor](skills/customer-story-extractor/) | You have happy customers and no proof a skeptical buyer can check |

### Compound: you cannot tell what worked

| Skill | Use it when |
| --- | --- |
| [gtm-dashboard-spec](skills/gtm-dashboard-spec/) | Nobody agrees what the numbers mean, and the weekly review ends without a decision |

## How they fit together

```
   REACH                CAPTURE              CONVERT              COMPOUND
   found by the         turned into          turned into          learned from
   right people         conversations        revenue              and repeated

   aeo-page-audit  -->  landing-page    -->  positioning     -->  gtm-dashboard
   founder-content      teardown             canvas               spec
   campaign-brief       outbound             icp-sharpener         |
        ^               sequence             sales-one-pager       |
        |                                    customer-story        |
        +------------------------------------------------------ ---+
                         what you learn changes what you say next
```

Most skills cross-reference the others in a **Related skills** section at the
bottom. `positioning-canvas` is the one worth running first if more than one
lever feels broken, because everything downstream inherits the claim it
produces.

## What these skills will not do

- They will not invent customer names, quotes, statistics, or case studies. If
  the evidence is missing, they say so and mark the claim unproven.
- They will not send anything. Every outbound skill stops at a human approval
  step by design.
- They will not tell you your product is differentiated when it is not.

That last one is deliberate. Skills that flatter you produce work that loses
deals later, in a room you are not in.

## Who made this

Built by [Varun Choraria](https://varunchoraria.com?ref=pipeline-skills) at
[Grow & Close](https://growandclose.com?ref=pipeline-skills), a GTM execution
studio for founder-led B2B SaaS. We ship one GTM priority end to end, tied to
one pipeline number.

If a skill gets you most of the way and you want the rest done properly,
[book a call](https://cal.com/varun-choraria/30min). If it produced something
wrong or weak, [open an issue](https://github.com/vcxcvii/pipeline-skills/issues)
with the input and the output. That is the fastest way to make these better.

## Contributing

Pull requests welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the quality bar
each skill has to clear.

## Licence

MIT. Use them commercially, fork them, ship them inside your own product. No
attribution required, though a link back is appreciated.
