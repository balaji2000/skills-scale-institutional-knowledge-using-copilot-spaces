# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## New / Expanded Personas

### Release Manager
- Responsibilities:
  - Coordinate release windows and sequencing across teams
  - Maintain and execute the release checklist (pre-release, deploy, post-release)
  - Verify staging and production smoke tests and coordinate rollbacks when needed
  - Communicate release status to stakeholders and support teams
- Typical Decisions:
  - Go/no-go for scheduled release based on readiness criteria
  - Whether to initiate a rollback when safety criteria are met
- Primary Collaborators:
  - PM, PdM, Developers, QA, Platform/SRE, Support
- How they interact with existing roles:
  - Works with PM/PdM to schedule releases and confirm acceptance criteria.
  - Coordinates with QA and Developers for validation and with Platform/SRE for deploy automation.


### Platform / SRE Engineer
- Responsibilities:
  - Maintain CI/CD pipelines, deployment automation, and platform reliability
  - Own observability, runbooks, and post-deploy health checks
  - Support production troubleshooting and rollback steps
- Typical Decisions:
  - Implementation choices for deployment automation and alerts
  - When to escalate platform incidents to on-call or broader incident response
- Primary Collaborators:
  - Developers, Release Manager, Security Liaison
- How they interact with existing roles:
  - Partner with Developers to implement safe deployment patterns and telemetry.
  - Assist Release Manager during deployments and rollbacks.


### Security Liaison
- Responsibilities:
  - Coordinate security reviews and threat assessments for releases
  - Ensure scanning, gating, and compliance checks are in place in CI
  - Escalate security incidents to Security on-call and capture mitigations
- Typical Decisions:
  - Whether a security finding blocks a release until resolved or mitigated
- Primary Collaborators:
  - Developers, PM, Platform/SRE, Product Lead, Security team
- How they interact with existing roles:
  - Work with Developers to remediate security issues and with Product/PM for required trade-offs.


### UX / Design Researcher
- Responsibilities:
  - Provide user research and usability validation
  - Contribute to acceptance criteria for UX-sensitive backlog items
  - Assist with design handoffs and usability testing during QA
- Typical Decisions:
  - Approve UX acceptance criteria and identify major UX risks
- Primary Collaborators:
  - PdM, Developers, QA
- How they interact with existing roles:
  - Collaborate with PdM in planning and with QA to validate UX acceptance.


### Data / Analytics Owner
- Responsibilities:
  - Define success metrics and own instrumentation and dashboards
  - Validate data quality and help interpret post-release metrics
  - Ensure telemetry is implemented for key success signals
- Typical Decisions:
  - Which metrics are used to declare success and how they are measured
- Primary Collaborators:
  - PdM, Developers, Platform/SRE
- How they interact with existing roles:
  - Work with PdM to confirm success metrics; with Developers to instrument and Platform/SRE to surface dashboards.


### Technical Program Manager (TPM) / Delivery Lead
- Responsibilities:
  - Coordinate cross-team dependencies and complex integrations
  - Maintain the risk & dependency register and milestone tracking for multi-team efforts
  - Remove blockers and align timelines for large initiatives
- Typical Decisions:
  - Adjust orchestration or timelines to manage cross-team capacity and dependencies
- Primary Collaborators:
  - PMs, Product Leads, Engineering Managers
- How they interact with existing roles:
  - Operate as the connector between multiple PMs/PdMs and engineering teams, particularly for integration work.

---

## Accountability Table (example)
For each persona add a short table with:
- Responsibilities: [short list]
- Typical Decisions: [short list]
- Primary Collaborators: [short list]

(Include these tables above for each persona to make responsibilities and handoffs explicit.)
