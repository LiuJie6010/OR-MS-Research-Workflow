# Theorem Interpretation

## Purpose

Turn formal results into credible Management Science body prose without weakening the math or overstating the claim. This is a subroutine of `management-science-writing.md`, not a replacement for the whole body-writing workflow.

## When to Use

Use after theorem, proposition, lemma, corollary, example, or numerical result statements, especially when the user asks for interpretation, intuition, managerial meaning, or section narrative. When the user is revising a body section, load this together with `management-science-writing.md`; when proof validity or claim status is uncertain, also load `proof-rigor.md`.

## Inputs Needed

- Formal statement and proof status.
- Assumptions and benchmark.
- Result type: equivalence, bound, monotonicity, convexity, structure, approximation, robustness, or counterexample.
- Intended managerial message.

## Procedure

For each result, write in this order:

1. Mathematical content. State exactly what the result proves.
2. Mechanism. Explain why it happens using the primitives of the model.
3. Economic meaning. Translate the result relative to the benchmark or alternative.
4. Managerial implication. State what the manager can decide, precompute, monitor, avoid, or prioritize.
5. Failure mode. Say what breaks when the condition fails or which complementary concern becomes important.

Use theorem register only for statements with clear primitives, feasible set, and conclusion. Use design-lens register for proxies, diagnostics, upper bounds, or informal prescriptions.

## Expected Output

Return:

- A calibrated interpretation paragraph.
- A claim-status note: theorem, proposition, corollary, example, or discussion.
- A warning if the intended managerial claim exceeds the formal result.

## Common Failure Modes

- Repeating the theorem in words without explaining mechanism.
- Hiding the benchmark.
- Calling a diagnostic an optimal policy.
- Presenting an order result as an exact equality.
- Omitting the failure mode.
