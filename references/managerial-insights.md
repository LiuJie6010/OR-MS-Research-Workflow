# Managerial Insights

## Purpose

Write post-result managerial paragraphs that are useful, credible, and tied to formal or numerical evidence. This is a subroutine of `management-science-writing.md`, not a separate paper-writing workflow.

## When to Use

Use after propositions, theorems, examples, numerical findings, robustness checks, and design-lens sections. When the implication is part of body-section prose, load this together with `management-science-writing.md`; when the implication comes from a formal result, also load `theorem-interpretation.md`.

## Inputs Needed

- Result statement or finding.
- Regime and assumptions.
- Mechanism.
- Benchmark or alternative policy.
- Practical decision object.

## Terminology Checkpoint

Apply `terminology-discipline.md`. Preserve the result's manuscript-defined names for regimes, mechanisms, policies, metrics, and decision objects. Do not create a new policy name, mechanism label, or managerial acronym to make the paragraph sound memorable. When no supported term exists, use neutral operational language and place any candidate name in a separate terminology-decision note.

## Procedure

Use the four-part paragraph template:

1. Regime. Name which setting or condition the result captures.
2. Mechanism. Explain why the result occurs.
3. Operational implication. Say what the manager can do and with which data or offline computation.
4. Failure mode or trade-off. Say what happens if the hypothesis fails or which complementary priority becomes important.

Prefer concrete operational verbs: precompute, monitor, cap, allocate, rebalance, screen, pool, reserve, prioritize, diagnose, approximate, or stress-test.

## Expected Output

Return one polished paragraph plus a short evidence note identifying which theorem, proposition, or experiment supports each sentence.

## Common Failure Modes

- Writing generic "this has important implications" prose.
- Omitting the failure mode.
- Giving a recommendation that is not supported by the result.
- Hiding whether the recommendation is offline design, real-time control, or diagnostic interpretation.
- Inventing a memorable policy or mechanism name that the manuscript or literature does not support.
