# Measurement Guide

## Start with the workflow

Do not begin with model metrics. Begin with a workflow that matters to the business, such as PR review, support resolution, or analyst turnaround.

For each workflow, define:

- the starting trigger
- the completion event
- the quality checkpoint
- the human review step
- the business outcome tied to success

## Source systems to inspect

Common sources include:

- ticketing systems
- Git platforms
- CRM or support platforms
- BI tools
- workflow orchestration tools
- internal copilot or chat logs
- audit and policy systems

## Minimum viable measurement loop

1. Capture when AI assistance was available.
2. Capture whether the user accepted, edited, or ignored the output.
3. Capture whether a human reviewer overrode the result.
4. Capture the workflow completion time and quality result.
5. Compare against baseline and a non-assisted control where possible.

## Recommended review cadence

- Weekly: operational changes, adoption trends, instrumentation gaps
- Monthly: business impact, target review, governance issues
- Quarterly: metric retirement, new workflow selection, scorecard redesign

## Common mistakes

- Measuring only AI usage and calling it impact
- Using self-reported time saved as the primary KPI
- Ignoring review and override behavior
- Mixing experimental and production workflows in one scorecard
- Optimizing speed without a paired quality safeguard

