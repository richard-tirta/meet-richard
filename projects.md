# Projects — 2025–2026

What I've been building recently. The repositories are private (production
systems and personal data), but the work is described here at the depth I
can share. Deeper walk-throughs available in conversation.

## Apple RFSAC — manufacturing dashboards + AI platform frontend (day job)

See [experience.md](experience.md) — critical interactive dashboards over
high-volume manufacturing data (Plotly/D3, scaled to 100M+ data points),
plus frontend work on an internal enterprise AI platform built against an
MCP integration boundary. NDA; described there at the depth I can share.

## Sutterfields — full digitization of a real retail business

The most complete demonstration of my range: I'm building the entire
digital operation for **Sutterfields**, a furniture/home-goods consignment
gallery — marketing site through back-office operations, all in production
with real daily users.

- **Marketing site** ([sutterfields.com](https://sutterfields.com)):
  Next.js, form pipelines with validation and email delivery, Meta
  Conversion API + GA4 server-side attribution, ISR-cached gallery.
- **Admin platform**: a full Outlook-integrated operations app (Microsoft
  Graph) — shared-inbox triage with **LLM-powered classification**,
  consignment intake with e-sign agreement flow, label printing, inventory
  projections from the legacy POS, buyer routing, and a web-attribution
  loop closing ad-spend back to accepted consignments.
- **Standalone sale app**: Entra-authenticated point-of-sale slice with
  role-based access on a shared Postgres (Neon).
- **AI in production**: model-tiering decisions (small models where they
  measurably suffice — validated by agreement testing against larger ones),
  vision-assisted item intake, throttling/cost control on an AI gateway.

Solo-built: schema, migrations, auth (hand-rolled MSAL + JWT sessions),
UI, integrations, deployment. The interesting part isn't any one feature —
it's that a real business runs on it.

## AI-powered career/interview practice hub (personal product)

A private Next.js app I built for my own interview readiness — and a
working showcase of LLM product engineering:

- **Generator/judge pipelines**: one model writes practice material
  (drills, quizzes, code-review exercises), a stronger model judges
  free-form answers against a structured rubric.
- **Spaced repetition** driven by actual miss history; difficulty dials;
  pre-generated hints; deliberate motivation-first UX.
- **PR-review training mode**: model-generated single-file diffs with
  planted defects, graded on severity triage (approve vs request-changes).
- **Architecture split** on principle: knowledge lives as markdown in git
  (edited through the GitHub Contents API from the deployed app), practice
  telemetry lives in Postgres. Async generation with background functions
  and graceful pending/failed states.
- Multi-provider: Anthropic models direct + OpenAI models via an AI
  gateway, with per-record model tagging for comparison.

## richardtirta.com — portfolio rebuild

Current-generation portfolio ([richardtirta.com](https://richardtirta.com)):
React Three Fiber / three.js scene work, audio-reactive visuals with a
build-time-baked synth bed (solving CPU contention between canvas and
audio), FPS probing with progressive canvas gating, and
**accessibility-first motion** (WCAG AA as the floor, not the ceiling).
Includes a [making-of](https://richardtirta.com/making-of) engineering
colophon.
