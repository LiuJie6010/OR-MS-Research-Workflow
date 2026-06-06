# Experiment Design

## Purpose

Design numerical experiments for OM/OR papers that support theory, illustrate mechanisms, test robustness, and communicate managerial insight.

## When to Use

Use for simulation plans, computational experiments, numerical sections, robustness checks, figure/table planning, and experiment narrative writing.

## Inputs Needed

- Main theoretical result and assumptions.
- Benchmark policies or designs.
- Parameters, instance classes, and uncertainty model.
- Intended managerial insights.
- Computational budget.

## Procedure

1. State the role of experiments: validate theory, illustrate mechanism, test robustness, compare benchmarks, or explore extensions.
2. Choose baselines that a referee would consider fair.
3. Define instance generation with parameter ranges and fixed seeds when appropriate.
4. Select metrics tied to the paper's claims: profit, cost, service, regret, approximation ratio, fill rate, waiting, utilization, or stability.
5. Include sensitivity checks around assumptions that theory fixes.
6. Use figures for mechanism and tables for robustness or summary comparisons.
7. Write the section so every experiment answers a named question.
8. Do not make causal or universal claims beyond the experiment design.

## Expected Output

Return:

- Experiment questions.
- Instance design.
- Baselines.
- Metrics.
- Figures/tables.
- Expected narrative role.
- Risk controls.

## Common Failure Modes

- Running many experiments without a question.
- Choosing weak baselines.
- Reporting only favorable cases.
- Showing robustness without explaining which assumption is being stressed.
- Making plots pretty but not interpretable.
