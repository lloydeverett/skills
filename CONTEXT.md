# Matt Pocock Skills

A collection of agent skills (slash commands and behaviors) loaded by Claude Code. Skills are organized into buckets. The work they plan and build lives as markdown files under the target repo's `docs/`.

## Language

**Spec**:
A feature's settled plan, written by `to-spec` to `docs/specs/<feature-slug>.md`.

**Ticket**:
One tracer-bullet slice of a build, written by `to-tickets` as its own file at `docs/tickets/<feature-slug>/<NN>-<slug>.md`, carrying a `Blocked by:` line and a `Status:` line (`open` or `done`).
_Avoid_: issue (this fork has no issue tracker)

**Decision ticket**:
A `wayfinder` unit: a file under `docs/maps/<effort-slug>/tickets/` holding a *question* whose resolution is a decision, not a slice of a build to execute. The **decision** qualifier is what keeps it distinct from an implementation **Ticket**; `wayfinder` introduces the term, then uses "ticket".

## Relationships

- A **Spec** is split into many **Tickets**, which share its slug
- A **Decision ticket** belongs to one wayfinder map (`docs/maps/<effort-slug>/map.md`)

## Flagged ambiguities

- "backlog" is not a domain term. Work lives in **Specs** and **Tickets**.
- "Issue tracker" (GitHub Issues, Linear, and similar) was the upstream storage for specs and tickets. Resolved in this fork: markdown files under `docs/` replace it.
