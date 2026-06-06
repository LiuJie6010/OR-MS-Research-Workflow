# Rigor and Consistency

## Purpose

Audit consistency across the whole paper: question, abstract, introduction, model, assumptions, theorem claims, proofs, experiments, and managerial insights.

## When to Use

Use for manuscript-wide checks, pre-submission audits, revision planning, or when the user asks whether the paper is coherent and rigorous.

## Inputs Needed

- Abstract and introduction.
- Model and assumptions.
- Main results and proofs.
- Experiment section.
- Managerial insights and conclusion.

## Procedure

1. Extract the paper promise from abstract and introduction.
2. Map each promised contribution to body evidence.
3. Check assumption visibility and consistency.
4. Check theorem/proposition statements against proof status.
5. Check numerical claims against implemented experiments.
6. Check managerial insights against formal or numerical support.
7. Check terminology consistency.
8. Flag unsupported, overstated, duplicated, or missing claims.

## Expected Output

Return a claim-evidence audit table with:

- Claim.
- Location.
- Supporting result or experiment.
- Status: supported, conditional, overstated, missing, or unclear.
- Required fix.

## Common Failure Modes

- Revising a paragraph locally while breaking the paper's global promise.
- Letting the introduction advertise an unimplemented numerical feature.
- Changing terminology between body and appendix.
- Forgetting assumptions in the abstract or managerial implications.
