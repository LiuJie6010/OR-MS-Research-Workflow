# Theorem Interpretation

## Purpose

Turn formal results into credible Management Science prose without weakening the math or overstating the claim. Use independently for a local interpretation, or with the body-writing workflow for broader prose revision.

## When to Use

Use when a result needs interpretation, intuition, managerial meaning, or section narrative. Load [proof rigor](proof-rigor.md) when validity or claim status is uncertain; interpretation alone does not require re-proving the result.

## Inputs Needed

- Formal statement and proof status.
- Assumptions and benchmark.
- Result type: equivalence, bound, monotonicity, convexity, structure, approximation, robustness, or counterexample.
- Intended managerial message.

## Terminology Checkpoint

Reuse the formal statement's terminology. Use [terminology discipline](terminology-discipline.md) for unsupported labels, naming proposals, or conflicts.

## Procedure

Cover the relevant elements in a coherent paragraph; adapt order and detail to the result and request:

1. Mathematical content. State exactly what the result proves.
2. Mechanism. Explain why it happens using the primitives of the model.
3. Economic meaning. Translate the result relative to the benchmark or alternative.
4. Managerial implication. State a supported decision or action when the result has one; a technical lemma may only support a later result.
5. Scope and failure mode. State where the guarantee applies. Describe failure outside its assumptions only with supporting analysis or evidence; lack of a guarantee does not imply failure.

Use formal language for proved statements with clear primitives, feasible set, and conclusion, including proved upper bounds. Label informal prescriptions or diagnostic interpretations as such rather than presenting them as guarantees.

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
- Claiming failure merely because a sufficient condition is not satisfied.
- Introducing an unsupported nickname or mechanism label that does not appear in the manuscript or identifiable literature.
