# product-roadmap-skill
# Roadmap Generator

> A Claude skill that turns a backlog, prioritization output, or rough brain dump into a structured, communicable product roadmap — with a sequencing rationale that survives a skeptical question.

Part of the [Cadboro Labs](https://cadborolabs.com) PM toolkit. Chains naturally from [feature-prioritization](https://github.com/brandonsgitstub) — scores in, sequenced roadmap out.

## What it does

A roadmap is a communication tool, not a backlog with dates stapled on. This skill makes the *logic* of the sequence legible, so a skeptical engineer or exec understands not just what's planned, but why this and why now.

- **Input-flexible** — works from a messy brain dump, a pasted backlog, customer themes, or a RICE prioritization output.
- **Three views** — Now / Next / Later (default), theme-based, or quarterly / time-boxed, with guidance on picking the right one for your audience.
- **Defensible by construction** — every committed item carries a *why-now*, its *dependency*, and a *success signal*, plus a sequencing rationale that names the through-line, the top calls, and what got deprioritized.
- **Guards against the classics** — the everything-is-Now trap, date theater on unscoped work, and hidden dependencies.

## Outputs

- **Roadmap** (`.md`) — the structured roadmap in your chosen view.
- **Sequencing rationale** — why things are ordered this way, what got pushed, and the assumptions a reader should challenge.
- **Optional timeline** (`.xlsx`) — a color-coded swimlane view for sharing with leadership.

## Install

```bash
claude skill install product-roadmap-skill
```

## Use

Just describe what you've got:

```bash
claude "Turn this backlog into a roadmap — our goal this half is activation"
claude "I ran a RICE prioritization, sequence it into a roadmap for my eng lead"
claude "Lay out a quarterly roadmap — we committed to ship SSO by end of Q4"
```

## What's inside

```
product-roadmap-skill/
├── SKILL.md                      # the skill
└── references/
    ├── roadmap-guide.md          # the three views, when to use each, anti-patterns
    ├── roadmap-template.md       # markdown structure for the roadmap + rationale
    └── timeline-spec.md          # layout spec for the optional .xlsx swimlane
```

## License

Open source. Free forever.

---

Built by [Brandon Gains](https://www.linkedin.com/in/brandon-gains/) · [Cadboro Labs](https://cadborolabs.com)
