# Management Science Writing

## Scope

Revise OM/OR main-body prose, result narratives, conclusions, and appendices so formal rigor supports a clear managerial story. Use [abstract writing](abstract-writing.md) or [introduction writing](introduction-writing.md) for those deliverables.

Work from the supplied section, audience, results, benchmarks, assumptions, proof status, and local style constraints. Preserve the shared research invariants in [SKILL.md](../SKILL.md); report only material missing context.

## Writing Decisions

- Make the managerial or economic question visible and explain the trade-off behind the central result.
- State what the result improves, matches, relaxes, or diagnoses relative to its benchmark.
- Explain the operational meaning of structural properties such as monotonicity, convexity, sparsity, or connectivity when relevant to the paragraph.
- Distinguish theorem-level guarantees from informal interpretation, proxies, diagnostics, and design suggestions. A rigorously proved bound is still a formal result; an unproved prescription based on it is not.
- Preserve constants, thresholds, asymptotic hypotheses, feasible sets, and comparison definitions.
- Check affected terminology and notation. Load [terminology discipline](terminology-discipline.md) for naming, conflicts, or provenance questions; preserve routine defined terms without repeating its full protocol.
- Use concise academic prose and concrete verbs. Avoid decorative novelty claims and vague praise. By default, avoid em dashes and semicolons in manuscript prose; follow explicit author style requests. Annotation and punctuation preferences are not approval gates.

## Conditional Supporting Guides

Load only when the local problem requires more detail:

- [Theorem interpretation](theorem-interpretation.md): mathematical content, mechanism, economic meaning, and supported implications of a result.
- [Managerial insights](managerial-insights.md): evidence for a recommendation, its regime, operational action, and limits.
- [Proof rigor](proof-rigor.md): uncertain validity, assumptions, constants, proof obligations, or boundary cases.

These are diagnostic lenses, not compulsory sections after every lemma. Explain a guarantee's scope without inventing a failure outside it, and do not add a managerial action that the result does not support.

## Output

Return the requested polished prose. Separately note material claim calibration, missing evidence, or notation and terminology decisions. Include a broader audit or detailed explanation only when requested or needed to understand a substantive change.

## Common Failure Modes

- Saying "optimal" without a feasible set or benchmark.
- Saying "same savings" when only same-order savings are proved.
- Presenting a design suggestion as a proved guarantee.
- Making the introduction promise more than the body supports.
- Renaming a defined object for stylistic variety or changing its meaning during polish.
