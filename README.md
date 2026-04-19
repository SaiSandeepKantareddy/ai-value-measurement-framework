# AI Value Measurement Framework

Most companies are measuring AI wrong. They track activity instead of outcomes:

- prompts sent
- chat volume
- story points
- lines of code
- hours saved without evidence

This framework helps teams measure AI in a way leaders can trust. It is designed for engineering, support, analytics, operations, and internal copilots.

## Why this exists

AI usage is easy to count. AI value is harder to prove.

This repo gives teams a practical way to answer:

- which AI workflows are creating measurable value
- which ones are creating activity without impact
- which ones should scale, be fixed, be paused, or be retired

## What this repo gives you

- a reusable KPI taxonomy for AI value measurement
- scorecards and metric-definition templates
- rollout playbooks for pilots and scaled adoption
- instrumentation guidance and event schemas
- governance and executive review templates
- decision rules for when to scale, fix, pause, or retire workflows

## Start in 60 seconds

- If you are a leader: start with [executive/one-page-ai-roi-summary.md](./executive/one-page-ai-roi-summary.md)
- If you are rolling out a pilot: start with [playbooks/30-day-pilot.md](./playbooks/30-day-pilot.md)
- If you are a manager: start with [playbooks/manager-playbook.md](./playbooks/manager-playbook.md)
- If you are implementing measurement: start with [instrumentation/measurement-guide.md](./instrumentation/measurement-guide.md)
- If you want the guided path: start with [start-here/README.md](./start-here/README.md)

## Who this is for

- CEOs, CIOs, CTOs, and business leaders
- AI platform and transformation teams
- engineering, support, analytics, and operations leaders
- managers running AI pilots in their teams
- internal tool and copilot builders

## Core idea

AI does not create value because people used it. AI creates value when it improves:

- adoption in the right workflows
- speed on meaningful work
- quality of outcomes
- throughput of completed work
- leverage per person or team
- risk and governance control

The framework is reusable across companies because the KPI categories stay mostly the same. What changes by company is:

- which workflows matter most
- which systems contain the source data
- what outcomes the business cares about

## Framework flow

```mermaid
flowchart LR
    A[Pick A Workflow] --> B[Define Baseline]
    B --> C[Instrument Events]
    C --> D[Measure Six Pillars]
    D --> E[Interpret Business Impact]
    E --> F{Decision}
    F -->|Scale| G[Expand To More Teams]
    F -->|Fix| H[Improve Workflow Or Guardrails]
    F -->|Pause| I[Stop Expansion]
    F -->|Retire| J[End Low-Value Pilot]
```

The six pillars are:

- adoption
- speed
- quality
- throughput
- leverage
- risk and governance

## The six pillars

### 1. Adoption

Measure whether AI is being used in the workflows where it should matter.
- weekly active AI users in target roles
- percent of eligible workflows using AI assistance
- repeat usage rate after first use
- team-level adoption by function

### 2. Speed

Measure time reduction in meaningful process steps, not vague effort claims.
- cycle time reduction
- median time to first draft
- mean time to resolution
- analysis turnaround time

### 3. Quality

Measure whether outcomes improved, not just whether work happened faster.
- rework rate
- defect escape rate
- first-contact resolution
- answer acceptance rate
- audit pass rate

### 4. Throughput

Measure whether the team can complete more useful work with the same capacity.
- tickets resolved per week
- analyst deliverables completed
- experiments shipped
- documents updated

### 5. Leverage

Measure whether teams can take on more scope or complexity without proportional headcount growth.
- output per team member
- additional workload absorbed
- ratio of assisted to unassisted completions
- manager span supported by AI-enabled workflows

### 6. Risk and Governance

Measure whether AI usage remains safe, reviewable, and aligned with policy.
- percent of AI outputs reviewed
- override rate
- policy exception count
- hallucination or factual error rate
- sensitive-data incident count

## Good measurement principles

- Start with a workflow, not a model.
- Compare against a baseline.
- Combine leading and lagging indicators.
- Pair speed with quality.
- Capture risk alongside upside.
- Add business interpretation, not just metric movement.

## What not to track

Avoid KPIs that reward visible activity instead of useful outcomes.

Common anti-patterns:

- raw chat volume
- prompts per employee
- Jira hours
- story points completed
- lines of code
- unverified time-saved claims
- number of models deployed

See [anti-patterns/README.md](./anti-patterns/README.md) for details.

## What is inside

- [start-here](./start-here/README.md): guided entry points by role
- [executive](./executive): one-page summaries and review questions
- [playbooks](./playbooks): pilot, rollout, and manager operating guides
- [templates](./templates): scorecards, metric definitions, and review templates
- [instrumentation](./instrumentation): event taxonomy and implementation guidance
- [integrations](./integrations/README.md): common enterprise system mappings
- [governance](./governance): review cadence, tiering, and metric policy
- [examples](./examples): function-specific scorecards
- [decision-rules](./decision-rules/README.md): scale, fix, pause, or retire logic
- [calculators](./calculators): ROI and prioritization starters

## Repository structure

```text
ai-value-measurement-framework/
  README.md
  start-here/
  maturity-model/
  executive/
  playbooks/
  integrations/
  governance/
  calculators/
  benchmarks/
  decision-rules/
  templates/
  examples/
  instrumentation/
  anti-patterns/
```

## How to use it

1. Pick one high-value workflow.
2. Define the baseline before AI intervention.
3. Choose one or two metrics from each relevant pillar.
4. Instrument the source systems that produce evidence.
5. Review weekly for operational learning and monthly for business impact.
6. Retire metrics that create bad incentives.

## Starter use cases

- Engineering: PR cycle time, escaped defects, review turnaround, deployment frequency
- Support: handle time, first-contact resolution, escalation rate, policy exception rate
- Analytics: time to insight, dashboard turnaround, revision count, decision adoption
- Operations: case processing time, backlog burn rate, exception handling, control breaches

## Design principles

- Track business outcomes over user activity.
- Prefer observed behavior over self-reported impact.
- Use simple scorecards before building complex dashboards.
- Treat human override and review as product signals, not nuisances.
- Separate adoption from value. High usage does not guarantee impact.

## Contributing

Contributions are most useful when they add:

- new metric definitions
- example scorecards for additional functions
- instrumentation patterns for common tool stacks
- case studies showing how teams interpreted results

## Suggested positioning

Use this framing when sharing the project:

> AI does not fail because models are weak. It fails because organizations do not know how to measure value.

## What makes this reusable

This repository is designed to be reusable because it includes:

- common KPI pillars that apply across functions
- templates that teams can adapt without redesigning the framework
- example scorecards for common workflows
- a shared instrumentation model
- governance and executive reporting layers
- role-based and maturity-based adoption paths

Measure AI like a business system, not a novelty.
