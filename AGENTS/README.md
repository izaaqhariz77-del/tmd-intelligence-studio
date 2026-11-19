# TMD Agents

Five independent AI agents for THE MARKET DOCTRINE. Each is a set of written instructions, not software: no code, no dependencies, no API keys. Any capable AI assistant can run them. In Claude Code they are also available as skills.

| Agent | Job | Writes drafts to | Claude Code skill |
|---|---|---|---|
| [TMD_INTELLIGENCE](TMD_INTELLIGENCE/) | Audience profiles, pain points, public conversation themes, content opportunities | `RESEARCH/audience/` | `/tmd-intelligence` |
| [TMD_AUTHORITY](TMD_AUTHORITY/) | Positioning, thought leadership, brand consistency reviews | `STRATEGY/` | `/tmd-authority` |
| [TMD_CONTENT_LAB](TMD_CONTENT_LAB/) | Threads posts, Instagram carousels, XAUUSD explainers, trading psychology | `CONTENT/<channel>/` | `/tmd-content-lab` |
| [TMD_MAGNET](TMD_MAGNET/) | Educational resources, voluntary enquiry journeys, landing page copy | `RESOURCES/` | `/tmd-magnet` |
| [TMD_PROSPECT_INTELLIGENCE](TMD_PROSPECT_INTELLIGENCE/) | Organises voluntary enquiries, consent and missing information; human review queue | Nothing in this repository | `/tmd-prospect-intelligence` |

## Ground rules for every agent

- **Drafts only.** No agent publishes, schedules, sends messages or contacts anyone. People approve and publish ([approval workflow](_shared/approval-workflow.md)).
- **No broker solicitation.** No account-opening, deposit or referral calls to action while the regulatory gate is closed. Coaching promotion is on hold.
- **No invented proof.** No performance, testimonials, credentials or regulatory claims beyond the verified facts register.
- **Two audience segments, kept separate:** PRIMARY (experienced, active traders) and SECONDARY (traders rebuilding after losses), with protections for the second.
- **No personal data in this repository.**

The full rules are in [`_shared/guardrails.md`](_shared/guardrails.md). It is the first file every agent reads.

## Shared files

| File | Purpose |
|---|---|
| [`guardrails.md`](_shared/guardrails.md) | Compliance rules, methodology facts, segments, classes, status snapshot |
| [`approval-workflow.md`](_shared/approval-workflow.md) | Statuses, gates, what counts as approval |
| [`quality-checklist.md`](_shared/quality-checklist.md) | Checks every output passes, and the checks block format |
| [`data-handling.md`](_shared/data-handling.md) | Personal data, consent, public conversations, retention |
| [`output-header.md`](_shared/output-header.md) | Header block and file naming for every output |
| [`integrations.md`](_shared/integrations.md) | Optional connectors and what each may do |

## How to run an agent

**Claude Code:** type the skill name and the task, for example:

```
/tmd-content-lab Threads, campaign voice, Sun 29 Nov 8:30am, Rule #30, SECONDARY, educational: plan before the session.
```

**Any other AI assistant:** paste `_shared/guardrails.md`, the agent's `AGENT.md` (plus any file its "Read first" list names), then the task.

Each agent's `README.md` lists its inputs and outputs. Each has worked examples in `examples/`.

## How the agents fit together

```
TMD_INTELLIGENCE ──opportunities──▶ TMD_CONTENT_LAB ──drafts──▶ Owner review ──▶ Publish (owner's instruction)
        │                                   ▲
        └──────pain points──────▶ TMD_MAGNET ──journeys──▶ TMD_PROSPECT_INTELLIGENCE ──review queue──▶ Owner
TMD_AUTHORITY ──positioning, pillars, consistency reviews──▶ all agents
```

The agents are independent: none needs another to run. Hand-offs are files.

## Maintaining the agents

- Change a shared rule once, in `_shared/`. Agents reference it rather than repeating it.
- When the owner changes a status (coaching hold, broker gate, voice), update `guardrails.md` §10 first.
- Bump the version line at the top of any file you change.
- To add an agent: copy one agent folder, rewrite `AGENT.md`, `CHECKS.md`, `README.md` and the examples, then add a wrapper in `.claude/skills/`.
