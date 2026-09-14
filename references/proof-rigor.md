# Proof Rigor

## Purpose

Check mathematical rigor for OM/OR theory papers, with special attention to claim-proof alignment and constants.

## When to Use

Use for theorem/proposition review, proof sketches, appendix writing, formal status decisions, and reviewer-style rigor critique.

## Inputs Needed

- Formal statement.
- Definitions, assumptions, and notation.
- Manuscript-defined technical terms and their definition locations.
- Proof or proof sketch.
- Any asymptotic regime, thresholds, constants, or benchmark result.

## Procedure

Preserve the statement's terms and definitions. Use [terminology discipline](terminology-discipline.md) for a substantive rename or unsupported or conflicting label.

1. Verify statement precision. Check quantifiers, feasible sets, parameter ranges, and edge cases.
2. Match proof to claim. Ensure the proof establishes the exact statement, not a nearby intuition.
3. Carry constants explicitly. Replace "small enough" or "large enough" with named thresholds where possible.
4. Distinguish per-element and total perturbations. Account for combinatorial factors.
5. Check dependencies. Each lemma should depend only on stated assumptions or prior results.
6. Check boundary cases. Include zero, equality, degeneracy, empty sets, symmetric cases, and limiting regimes when relevant.
7. Compare parallel results quantitatively. If thresholds differ, explain the mechanism rather than hiding the difference.
8. Recommend formal status based on what is proved and its role in the paper. A lemma, proposition, or theorem can all be rigorous; do not weaken a valid result merely because it is peripheral, or silently alter assumptions or conclusions to hide a proof gap.

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
- Renaming a formal object or result inside a proof without reconciling the definition and every manuscript occurrence.
