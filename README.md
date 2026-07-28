# Pocket Agent Starter Skills

Most agent skills are written for developers. These 30 are written for business owners: email, sales, research, operations, decisions, and the writing voice that ties it all together.

They ship inside [Pocket Agent](https://aipocketagent.com) as the Starter Pack every workspace gets seeded with. The files use the open [Agent Skills](https://agentskills.io) format, so they load into Claude Code, Cursor, Gemini CLI, or any runtime on the [client list](https://agentskills.io/clients) exactly as they load into Pocket Agent. We extracted them from the product and published them here for the AI agent community to use and remix.

## What's inside

Each skill is one technique, taught the same way: the move, five concrete rules, a paired "do this, not that" example, and why it works. No filler sections.

### `skills/voice/`: how the agent writes

- `lead-with-the-action`: put the claim, finding, or ask in the first sentence, then explain.
- `specific-over-generic`: a name, a number, a date in every claim; kill the vague version.
- `dont-be-a-chatbot`: no throat-clearing, no hedged enthusiasm, no chatbot filler.
- `honest-hedging`: commit to a read; flag real uncertainty instead of hedging everything.
- `write-like-the-user`: match the owner's own vocabulary and cadence, not generic SaaS-speak.

### `skills/email/`: drafts that get replies

- `cold-intro-structure`: a cold intro built around the recipient's problem, not your company.
- `quote-follow-up`: re-send the value, not a nudge; add one honest reason to decide now.
- `customer-reply-tone-match`: mirror the customer's register before answering their question.
- `subject-line-not-filtered`: subject lines that read like a person, so they get opened.
- `boundary-setting-decline`: say no cleanly without burning the relationship.

### `skills/sales/`: from lead to close

- `lead-qualification`: sort a lead as real, later, or never before spending time on it.
- `discovery-call-note-capture`: capture the buyer's words, stakes, and objections from a call.
- `objection-handling`: answer the objection under the objection, not the surface one.
- `proposal-drafting-framework`: turn call notes into a proposal in the buyer's own terms.
- `stack-the-deck-close`: restack everything they get right before the price, then ask.

### `skills/research/`: findings you can act on

- `source-verification`: every claim points at its source; unverified stays flagged as unverified.
- `competitor-pricing-extract`: pull a competitor's real pricing with dates and receipts.
- `customer-voice-extract`: mine reviews and calls for quotes in the customer's own words.
- `tactic-extraction`: pull the usable plays out of long content, skip the fluff.
- `vertical-landscape-scan`: a one-page market scan: players, prices, gaps.

### `skills/operations/`: the daily grind, handled

- `inbox-triage`: sort the inbox into now, this week, archive, delegate.
- `quote-drafting-from-notes`: turn messy field notes into a clean quote.
- `vendor-invoice-categorization`: file invoices consistently so the books stay usable.
- `project-scaffolding`: turn a vague goal into milestones and tasks someone can actually run.
- `end-of-day-reflection`: a short end-of-day read: what shipped, what moved, what's stuck.

### `skills/decisions/`: pressure-test before you commit

- `three-option-framing`: three real options with trade-offs, never a single take-it-or-leave-it.
- `devils-advocate-first-pass`: argue the other side before presenting a plan.
- `pre-mortem`: assume it already failed, write down why, fix the top causes now.
- `load-bearing-assumption`: name the one assumption the whole plan rests on.
- `reversibility-check`: size the decision by how hard it is to undo.

## Install

**Claude Code.** Copy any skill directory into `~/.claude/skills/` (personal) or `.claude/skills/` in a project:

```bash
git clone https://github.com/cwhited26/pocket-agent-starter-skills.git
cp -r pocket-agent-starter-skills/skills/email/quote-follow-up ~/.claude/skills/
```

Docs: [code.claude.com/docs/en/skills](https://code.claude.com/docs/en/skills)

**Cursor.** Copy a skill directory into `.cursor/skills/` in your project:

```bash
cp -r pocket-agent-starter-skills/skills/sales/objection-handling .cursor/skills/
```

Docs: [cursor.com/docs/context/skills](https://cursor.com/docs/context/skills)

**Pocket Agent.** Nothing to install. These seed into your workspace's brain as the Starter Pack, and your agent loads them when the work calls for one. [aipocketagent.com](https://aipocketagent.com)

**Anything else.** Any runtime on the [agentskills.io client list](https://agentskills.io/clients) reads the same directory layout. Point it at a skill directory and go.

## Format

Every skill is a directory containing a single `SKILL.md`: spec-standard frontmatter (`name`, `description`, `license`, `metadata`) followed by the instructions. CI validates every skill against the [Agent Skills specification](https://agentskills.io/specification) with [`skills-ref`](https://github.com/agentskills/agentskills/tree/main/skills-ref) on every push, so a broken skill can't merge.

## License

MIT. These were extracted from Pocket Agent's Starter Pack and are shared for the AI agent community to remix. Keep them, change them, ship them inside your own agents. A link back to [aipocketagent.com](https://aipocketagent.com) is appreciated, never required.
