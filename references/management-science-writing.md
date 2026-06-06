# Management Science Writing

## Purpose

Revise OM/OR main-body prose so formal rigor serves a clear managerial story. Use this as the parent writing workflow for Management Science, Operations Research, Manufacturing & Service Operations Management, Production and Operations Management, and similar outlets.

## When to Use

Use for main body sections, theory sections, result interpretation, design sections, conclusions, appendices, abstract drafting after the body is clear, and paper-level style calibration.

Do not use this file as the full introduction architecture. For introductions, load `introduction-writing.md` after the body, contribution list, and roadmap are reasonably stable.

## Integrated Subroutines

This file controls the overall body-writing taste. Load the specialized files only when the local writing problem needs their structure:

- Load `theorem-interpretation.md` when a theorem, proposition, lemma, corollary, example, structural result, bound, or numerical result needs interpretation. Use it to turn formal content into mathematical content, mechanism, economic meaning, managerial implication, and failure mode.
- Load `managerial-insights.md` when a paragraph must become an evidence-tied managerial implication or operational recommendation. Use it to check regime, mechanism, action, and failure mode.
- Load `proof-rigor.md` when the paragraph's claim status depends on assumptions, constants, proof obligations, boundary cases, or whether the result is theorem-level versus design-lens prose.

If the draft contains a formal result with no mechanism or failure mode, invoke theorem interpretation. If the draft contains a practical recommendation with no supported action or regime, invoke managerial insights. If both are missing, invoke both subroutines before polishing the prose.

## Inputs Needed

- Target section and audience.
- Existing draft or outline.
- Main result, benchmark, assumptions, and proof status.
- Claimed managerial implication.
- Local style constraints, if any.

## Procedure

1. Start from the managerial problem. State the economic question before the technique.
2. Keep the benchmark visible. Say what the result improves, matches, relaxes, or diagnoses.
3. Make the trade-off explicit. Good OM/OR writing shows tension, not only improvement.
4. Translate structure into value. For structural properties such as monotonicity, convexity, sparsity, connectivity, or overlap, explain operational meaning.
5. Audit the local result narrative. After each theorem or finding, check whether the prose explains what it says, why it happens, why a manager should care, and what fails if assumptions fail. If not, use the theorem interpretation subroutine.
6. Audit the managerial paragraph. Check whether each recommendation names the regime, mechanism, operational action, and failure mode. If not, use the managerial insights subroutine.
7. Match claim status to proof status. Use theorem, proposition, corollary, example, discussion, or design lens according to what is actually proved.
8. Preserve mathematical precision. Keep explicit constants, thresholds, asymptotic hypotheses, feasible sets, and benchmark definitions.
9. Use human prose. Avoid decorative openers, vague adjectives, overexcited novelty claims, em dashes, semicolons, and generic AI phrasing.
10. Lock one term per concept across introduction, body, appendix, figures, and captions.

## Expected Output

Return polished prose plus a short note with:

- Claim calibration.
- Missing evidence or missing assumptions.
- Benchmark visibility.
- Theorem-to-insight quality.
- Subroutine used, if any: theorem interpretation, managerial insights, or proof rigor.
- Local style risks.

## Common Failure Modes

- Starting from the model technique instead of the managerial question.
- Adding managerial implications only at the end.
- Saying "optimal" without a formal feasible set.
- Saying "same savings" when only same-order savings are proved.
- Treating a design lens as a theorem.
- Hiding the benchmark.
- Making the introduction promise more than the body proves.
- Treating theorem interpretation or managerial insight as isolated add-ons instead of part of the body narrative.
