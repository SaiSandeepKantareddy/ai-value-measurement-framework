# Engineering Example Scorecard

## Workflow

Pull request creation, review, and merge for product engineering teams using AI coding assistants.

## Example metrics

| Pillar | Metric | Baseline | Target | Example interpretation |
| --- | --- | --- | --- | --- |
| Adoption | % of eligible engineers using AI weekly | 18% | 55% | Adoption is a gating metric, not proof of impact |
| Speed | Median PR cycle time | 46 hours | 34 hours | Reviews and revisions are moving faster |
| Quality | Escaped defect rate | 3.1% | <=3.1% | Speed gains are only valuable if quality holds |
| Throughput | Merged PRs per engineer per month | 7.4 | 8.5 | More completed work with the same team size |
| Leverage | % of low-complexity tasks completed without senior intervention | 22% | 40% | Senior engineers can focus on harder problems |
| Risk/Governance | % of AI-generated code changes reviewed before merge | 91% | 99% | Review coverage protects against silent regressions |

## Notes

- Do not use lines of code as a success metric.
- Separate assisted changes from non-assisted changes when possible.
- Track override or discard behavior because it often reveals quality gaps in suggestions.

