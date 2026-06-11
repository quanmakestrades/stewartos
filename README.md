# StewartOS

StewartOS is a private operator system for running a small AI-enabled company from a phone-first command surface.

This repo is the public, sanitized version. It explains the operating model without exposing the live workspace, memories, credentials, cron payloads, message routing, customer data, family data, or production configuration.

## What StewartOS Does

- Routes chat requests into product, engineering, content, finance, and operations workflows.
- Gives specialized AI agents clear roles instead of letting every agent do everything.
- Keeps durable project memory in files so work can survive session resets and context limits.
- Uses GitHub as the source-of-truth layer for code, docs, and public credibility.
- Separates public showcase material from private operator state.

## Agent Model

StewartOS treats agents like a small team:

- Coordinator: triage, summaries, reminders, and routing.
- Engineering: code, repos, deploys, debugging, and product implementation.
- Finance/Ops: financial recovery, operational checks, and business workflow support.
- Review/Repair: recurring audits, issue discovery, and bounded repair passes.

## Privacy Boundary

The real StewartOS workspace is private. This public repo only contains sanitized patterns and architecture notes.

Not included here:

- personal memory files
- real chat IDs or routing config
- credentials, tokens, or `.env` files
- cron payloads or live automation state
- family, client, inbox, calendar, or customer data
- unreleased business strategy

## Repository Map

- [`docs/architecture.md`](docs/architecture.md): high-level system shape
- [`docs/github-policy.md`](docs/github-policy.md): public/private repo rules

## Status

This is a showcase repo, not the production system. The useful public lesson is the operating pattern: keep the public architecture legible, keep the private state private, and version the real work deliberately.
