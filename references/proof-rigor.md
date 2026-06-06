# Proof Rigor

## Purpose

Check mathematical rigor for OM/OR theory papers, with special attention to claim-proof alignment and constants.

## When to Use

Use for theorem/proposition review, proof sketches, appendix writing, formal status decisions, and reviewer-style rigor critique.

## Inputs Needed

- Formal statement.
- Definitions, assumptions, and notation.
- Proof or proof sketch.
- Any asymptotic regime, thresholds, constants, or benchmark result.

## Procedure

1. Verify statement precision. Check quantifiers, feasible sets, parameter ranges, and edge cases.
2. Match proof to claim. Ensure the proof establishes the exact statement, not a nearby intuition.
3. Carry constants explicitly. Replace "small enough" or "large enough" with named thresholds where possible.
4. Distinguish per-element and total perturbations. Account for combinatorial factors.
5. Check dependencies. Each lemma should depend only on stated assumptions or prior results.
6. Check boundary cases. Include zero, equality, degeneracy, empty sets, symmetric cases, and limiting regimes when relevant.
7. Compare parallel results quantitatively. If thresholds differ, explain the mechanism rather than hiding the difference.
8. Decide formal status. Demote results that are useful but not central or not clean enough for theorem status.

## Expected Output

Return:

- Rigor findings ordered by severity.
- Missing assumptions or undefined objects.
- Claim-proof mismatch notes.
- Suggested revised statement or proof obligation.
- Formal status recommendation.

## Common Failure Modes

- Proving only sufficient conditions while stating equivalence.
- Losing constants in perturbation or asymptotic arguments.
- Treating borrowed proof machinery as a new contribution.
- Ignoring equality cases.
- Using "optimal" without specifying the feasible set.
