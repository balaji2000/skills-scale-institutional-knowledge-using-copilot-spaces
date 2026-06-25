# OctoAcme Project Management Docs — README

## What this is
A single landing page that summarizes OctoAcme's project management processes and provides direct links to the canonical process documents in this folder. This README is intended to improve discoverability, accelerate onboarding, and serve as a small index that points readers to the full, detailed process documents.

OctoAcme runs projects with a lightweight, iterative approach that moves work through a visible project board (Backlog → Ready → In Progress → In Review → QA → Done) and emphasizes small, reviewable increments. Initiation requires a one‑pager to capture the problem, goals, success metrics, and stakeholders. Planning turns an approved initiative into a prioritized backlog with clear acceptance criteria, estimates, a Definition of Done, and a release plan. Execution focuses on frequent team rhythm (standups, weekly delivery syncs, demos) and clear escalation paths for blockers.

Roles and responsibilities are explicit: Product Managers define outcomes and success metrics; Project Managers coordinate schedules, risks, and stakeholder communications; Developers implement features, tests, and documentation; QA validates acceptance and quality; and stakeholders provide approvals and inputs. Each project should name a PM and Product Lead and keep core artifacts—one‑pagers, roadmaps, risk registers, and retrospectives—up to date.

Quality assurance is integrated across the lifecycle. Developers write unit and integration tests, CI runs tests, linters and security scans, and smoke or end‑to‑end checks validate critical flows before release. Releases follow a checklist (staging verification, automated pipelines where possible, post‑deploy checks) and include rollback and incident playbooks. Retrospectives capture learnings and convert them into action items tracked in the backlog to support continuous improvement.

## Documents
- [Project Management Overview](./octoacme-project-management-overview.md) — high-level principles, roles, and lifecycle
- [Project Initiation Guide](./octoacme-project-initiation.md) — one-pager template, initiation checklist, decision gate
- [Project Planning](./octoacme-project-planning.md) — backlog, estimation, release plan, risk register guidance
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — team rhythm, workflows, QA, reporting, blocker escalation
- [Release & Deployment](./octoacme-release-and-deployment.md) — release types, deployment checklist, rollback playbook
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — risk register, communication templates, escalation paths
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — running retros, tracking actions
- [Roles & Personas](./octoacme-roles-and-personas.md) — role summaries and responsibilities

## How to use
- Link this README from project charters and the repo root to help new contributors find process guidance quickly.
- Keep each document in docs/ as the canonical source for that topic; this README should remain a concise index rather than the complete source of process detail.
- When process changes are proposed, update the relevant doc and consider updating this README if new documents are added or filenames change.

## Notes
- This README intentionally keeps summaries short and links to the full documents for details, templates, and checklists.
- For Copilot Spaces integration: add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as contextual sources.
