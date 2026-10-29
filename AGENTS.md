# AGENTS.md

Instructions for AI coding agents (Claude Code, Codex, others) working in this repo.

Last updated: 2026-10-29

## What this repo is

A public, portable AI operating system for people who orchestrate Claude. It is mostly Markdown: reusable agent patterns, one-time recipes, engineering guides, and a catalog of the `localwolfpackai` GitHub estate. Nothing runs from inside this repo; patterns are copied into other repos.

## Layout

- `patterns/` — drop-in agent setups. Each has a README, working code, an install path, and source credit (rules in `patterns/README.md`)
- `recipes/` — step-by-step walkthroughs
- `guides/` — engineering standards, kept as reference
- `docs/` — operating model, workflows, and dated repo-salvage findings
- `REPO-CATALOG.md` — status and destination of every repo in the estate
- `REPO-CLEANUP-QUEUE.md` — salvage, naming, and consolidation decisions waiting on the owner
- `CHANGELOG.md` — shipped versions and what is queued next

## Rules

- Every file runs or reads as finished. No stubs, placeholders, or empty folders for future work.
- Fewer files, not more. Update the doc that owns a topic instead of adding a new one; never create backup copies.
- Docs match disk. If a README names a folder that does not exist, fix the README.
- Repo renames, archives, and deletions are never automatic. Record them in `REPO-CLEANUP-QUEUE.md` for the owner to approve.
- Credit the source of any adapted pattern.
- Plain, specific writing. No emojis, no "delve", no "leverage".
- No secrets. Example settings go in `.env.example`; `.env` files stay ignored.

## Git

- Work on a feature branch and open a PR. The owner merges to `main`.
- Add a `CHANGELOG.md` entry for anything a reader would notice.
