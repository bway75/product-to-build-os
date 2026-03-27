# Setup Guide

This is the **product-to-build OS** — a baseline template for starting any new software project with a structured product, engineering, and governance workflow.

Read this first. It tells you what this repo is, how to use it to start a new project, and how to rebuild your environment on a new machine.

---

## What This Repo Is

A reusable operating system for AI-assisted product development. It defines:
- A canonical role model (Brian, Mason, Kade, Ledger, Case)
- A product-to-engineering delivery sequence
- Sprint execution, validation, and governance workflows
- Templates for all required project artifacts

It is a **template repo**, not a working project. Every real project is a separate repo that instantiates this OS.

---

## Starting a New Project

1. Create a new repo for the project
2. Follow `docs/process/PROJECT_BOOTSTRAP_CHECKLIST.md` — it walks through every file to copy, adapt, and instantiate
3. Do not start sprint work until the Ready-To-Execute check passes

---

## Rebuilding Your Environment on a New Machine

Machine setup is documented in your private **personal-process** repo (`FRESH_MACHINE_SETUP.md`). That file is kept separate from this public repo since it contains personal account details, specific applications, and connector configurations.

If you do not have access to that file, the core steps are:
1. Install Homebrew, Git, and Claude Code
2. Clone your repos into `~/Repository/GitHub/`
3. Install and configure Cowork (Claude desktop app)
4. Connect your Cowork connectors and plugins

---

## Key Files in This Repo

| File | Purpose |
|------|---------|
| `AGENT_MODEL.md` | How AI roles work together |
| `BRIAN.md` | Product authority role definition |
| `MASON.md` | Engineering execution role definition |
| `KADE.md` | Technical lead / governance role definition |
| `LEDGER.md` | Documentation and process role definition |
| `CASE.md` | Validation and QA role definition |
| `docs/process/PROJECT_BOOTSTRAP_CHECKLIST.md` | Step-by-step guide to instantiate this OS in a new project |
| `docs/process/ENGINEERING_WORKFLOW.md` | Branching, gates, TDD, and sprint completion rules |
| `docs/process/DEFINITION_OF_DONE.md` | Minimum standard before a sprint closes |
| `docs/process/AGENT_RULES.md` | Role boundaries and escalation rules |
| `docs/templates/` | All artifact templates (sprint spec, worklog, decisions log, etc.) |

---

## Keeping Projects in Sync with This OS

When a process improvement is made in a live project (like `internal_instance_explorer`), evaluate whether it should flow back here so future projects inherit it.

Sync checklist:
- [ ] Is the change generic enough to apply to any project?
- [ ] Does it belong in a process doc, a template, or both?
- [ ] Update the relevant file in this repo and commit
- [ ] Note the sync in `AI_WORKLOG.md`
