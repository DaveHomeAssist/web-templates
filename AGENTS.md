# AGENTS.md

Inherits root rules from `/Users/daverobertson/Desktop/Code/AGENTS.md`.

## Project Overview

Collection of reusable HTML layout templates and reference pages. Includes a home automation map, layout decision matrix, directory index, phase roadmap, status board, live event gear map, and prompt engineering reference. Used as starting points for new projects across the ecosystem.

## Stack

- Static HTML + CSS (one file per template)
- No build step, no framework
- Shared assets directory

## Key Decisions

- Each template is a standalone HTML file
- Templates serve as reference implementations for layout patterns
- Icons and Security directories contain specialized assets and reference pages

## Issue Tracker

| ID | Severity | Status | Title | Notes |
|----|----------|--------|-------|-------|

## Session Log

[2026-03-18] [WebTemplates] [docs] Add AGENTS baseline
[2026-06-10] [WebTemplates] [feat] Add layout_annotated_review.html — two-view review / issue-register pattern (filterable priority cards + margin-annotated source); catalog now lists 9 built layouts

## Status naming

Name work with one string everywhere (chat status title, session title, Notion
Status Check Runs "Human Name"):

`Project | 🚦 | Phase | Title → state, reason | MM-DD`

- 🚦: 🟢 complete and verified · 🟡 partial · 🔴 not started, blocked or failed · ⚪ unverifiable.
  Add ⏳ scheduled, 🙋 awaiting Dave or 🚧 blocked to 🟡/🔴/⚪, never to 🟢.
- Phase: Research, Design, Build, Audit or Scheduled. MM-DD: date of the latest light change.
- Every light change gets a new name: a `RENAME:` line in chat and the Notion row updated.
- Canonical source: https://github.com/DaveHomeAssist/skills/blob/master/status-naming.md
