# Rigor and Consistency

## Purpose

Audit consistency across the whole paper: question, abstract, introduction, model, assumptions, theorem claims, proofs, experiments, exposition, terminology, grammar, and managerial insights. For pre-submission review, perform a section-by-section audit and maintain a verification log. Do not mark any item as clean or verified unless the relevant text, proof, table, figure, cross-reference, or experiment claim has actually been checked.

## When to Use

Use for manuscript-wide checks, pre-submission audits, revision planning, or when the user asks whether the paper is coherent and rigorous.

## Inputs Needed

- Abstract and introduction.
- Model and assumptions.
- Main results and proofs.
- Experiment section.
- Managerial insights and conclusion.
- Appendix or electronic companion proofs.
- Current manuscript files, or extracted text with stable section and line references.
- Author style constraints, terminology preferences, and target journal.

## Procedure

Use two levels of audit.

### A. Global Claim-Evidence Audit

1. Extract the paper promise from abstract and introduction.
2. Map each promised contribution to body evidence.
3. Check assumption visibility and consistency.
4. Check theorem/proposition statements against proof status.
5. Check numerical claims against implemented experiments.
6. Check managerial insights against formal or numerical support.
7. Check terminology consistency.
8. Check definition-before-use. Flag any symbol, theorem label, assumption, model object, or technical concept used before it is defined in the manuscript.
9. Flag unsupported, overstated, duplicated, or missing claims.

### B. Pre-Submission Review Pass

Use this when the user asks for pre-submission review, final polish, full-manuscript checking, or a Management Science submission readiness audit.

1. Create a review log before editing. Include paper title, target journal, review date, manuscript files inspected, and whether line numbers are exact or approximate.
2. Do an initial full read-through and log obvious issues as `PRE.01`, `PRE.02`, etc. Do not fix silently.
3. Review the manuscript section by section. Use passes such as Abstract and Introduction, Literature Review, Model and Main Results, each technical-result section, Numerical Study, Conclusion, and E-Companion Proofs. Adapt names to the actual manuscript.
4. Within each pass, separate findings into Writing Quality, Technical Correctness, and Exposition. Writing Quality includes grammar, terminology, notation consistency, undefined notation or concepts, cross-reference style, caption-text mismatch, and informal phrasing.
5. For technical sections, check theorem/proposition statements against proof logic, assumptions, notation, boundary cases, constants, equations, algorithms, and examples. Record positive verifications only when the check was actually done.
6. For experiments, check that claims match implemented designs, baselines, tables, captions, parameter names, figures, and robustness results. Do not accept an introduction or abstract promise unless the experiment section supports it.
7. Run a global consistency sweep after section passes. Include notation consistency, terminology consistency, cross-reference and label consistency, capitalization of formal elements, citation-year or publication-status concerns, and table/figure naming consistency.
8. Reconcile pre-read issues with the systematic pass. If a pre-read issue is fixed or reclassified, point to the later issue ID.
9. Produce summary statistics by category and status. Exclude positive "Verified" technical checks from issue counts unless they required a fix.
10. End with low-confidence or author-decision items for coauthor review.

## Verification Discipline

- Use IDs that encode location: `S1.01` for Section 1 issue 1, `S9.03` for E-Companion issue 3, and `G10.01` for global sweep issues.
- Use types: Grammar, Terminology, Technical, Exposition, Notation, Cross-reference, Citation, Table/Figure, Experiment.
- Use confidence levels: High for objective or directly verified issues, Medium for likely but context-sensitive issues, Low for author judgment or taste.
- Use statuses: Identified, Fixed, Deferred, Author Decision Needed, Verified, Clean, No action needed.
- Reserve `Verified` for technical claims, proofs, algorithms, or references that were checked in substance.
- Reserve `Clean` for a completed sweep with no issue found.
- If the manuscript files are incomplete, say exactly which checks could not be guaranteed.
- When fixing text, preserve a log entry with the original problem, the fix, and the status. Do not replace the audit with a vague assurance.
- When only reviewing, not editing, use `Recommended fix` rather than `Fixed`.
- Use approximate line numbers only when stable exact line numbers are unavailable, and label them as approximate.

## Expected Output

Return either a claim-evidence audit table or a pre-submission review log.

For claim-evidence audit, include:

- Claim.
- Location.
- Supporting result or experiment.
- Status: supported, conditional, overstated, missing, or unclear.
- Required fix.

For pre-submission review, use this report structure:

1. Pre-Submission Review Log header.
2. Review Structure and status definitions.
3. Pass-by-pass section audit with tables.
4. Global Consistency Sweep.
5. Issues Found During Initial Read.
6. Summary Statistics.
7. Low-Confidence Items for Co-Author Review.

## Common Failure Modes

- Revising a paragraph locally while breaking the paper's global promise.
- Letting the introduction advertise an unimplemented numerical feature.
- Changing terminology between body and appendix.
- Forgetting assumptions in the abstract or managerial implications.
- Marking a proof as verified after only reading the theorem statement.
- Declaring terminology clean without searching or checking variants across the whole manuscript.
- Treating grammar polish as a substitute for technical rigor.
- Counting "no issue found" entries as fixed issues.
- Forgetting the appendix or electronic companion when the main text relies on deferred proofs.
- Reporting guaranteed status without naming what was inspected.
- Using notation, theorem labels, assumptions, or concepts before they are defined.

## Optional Full Example

If the user asks for the author's pre-submission review style, load `references/pre-submission-samples/pre-submission-review-log.md`. Use it as a structural example, not as reusable findings.
