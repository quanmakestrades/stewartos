# Architecture Overview

StewartOS is organized around a few simple boundaries:

## Operator Surface

The primary interaction model is chat-first. Requests arrive through a human-facing channel and are routed to the right agent or project workflow.

## Agent Roles

- Coordinator: triage, reminders, summaries, and cross-project routing.
- Engineering: code, repos, deploys, debugging, and product implementation.
- Finance/Ops: recovery plans, operational checks, and financial workflows.
- Review/Repair: scheduled checks, issue discovery, and bounded fixes.

## Memory

Agents use a file-backed memory pattern:

- Daily notes capture raw operational context.
- Long-term notes preserve durable decisions and lessons.
- Project reports preserve task-specific evidence and next steps.

The public pattern is shareable. The actual memory files are private.

## Project Surfaces

Projects are expected to have:

- A source repository.
- A deployment target when applicable.
- A short operational README.
- Clear rules for secrets, data, and generated artifacts.
- A human-facing status or approval surface when useful.

## Safety Boundary

The public StewartOS pattern avoids publishing:

- Secrets or tokens.
- Personal messages, emails, calendar data, or family context.
- Client data or unreleased strategy.
- Live routing identifiers.
- Production config.

