# Rigor and Consistency

## Purpose

Audit consistency across the whole paper: question, abstract, introduction, model, assumptions, notation, theorem claims, proofs, experiments, exposition, terminology, grammar, and managerial insights. For pre-submission review, perform a section-by-section audit and maintain a verification log. Do not mark any item as clean or verified unless the relevant text, proof, table, figure, cross-reference, notation use, terminology use, or experiment claim has actually been checked.

## When to Use

Use for manuscript-wide checks, pre-submission audits, revision planning, or requested cross-section consistency checks. Match coverage to the request: local polish does not require the full pre-submission workflow. Missing files limit verification claims, not work on available material.

## Inputs Needed

- Abstract and introduction.
- Model and assumptions.
- Main results and proofs.
- Experiment section.
- Managerial insights and conclusion.
- Appendix or electronic companion proofs.
- Current manuscript files, or extracted text with stable section and line references.
- Author style constraints, notation preferences, terminology preferences, and target journal.

## Procedure

Use two levels of audit.

### A. Global Claim-Evidence Audit

1. Extract the paper promise from abstract and introduction.
2. Map each promised contribution to body evidence.
3. Check assumption visibility and consistency.
4. Check theorem/proposition statements against proof status.
5. Check numerical claims against implemented experiments.
6. Check managerial insights against formal or numerical support.
7. For a full consistency audit, build a notation and terminology ledger with definitions, variants, and unresolved decisions. For a scoped review, inspect affected definitions and uses. Use [terminology discipline](terminology-discipline.md) for provenance and naming decisions.
8. Check notation consistency: the same symbol denotes the same object, each object has one primary symbol, and new symbols are defined before use.
9. Check that manuscript terms are used consistently and no unsupported or pending name has been adopted.
10. Flag undefined notation or concepts needed to understand a claim. A plain-language preview or resolvable forward reference is acceptable when it does not depend on unexplained notation.
11. Flag unsupported, overstated, duplicated, or missing claims.

### B. Pre-Submission Review Pass

Use this for a requested full pre-submission review, full-manuscript check, or submission readiness audit. "Final polish" alone follows the scope of the supplied text and request.

1. Maintain a review log as issues are found and edits are made. Include paper title, target journal if known, review date, manuscript files inspected, and whether line numbers are exact or approximate.
2. Read the available manuscript and record issues with stable IDs. A separate preliminary pass is optional; do not delay authorized fixes to complete duplicate passes.
3. Review the manuscript section by section. Use passes such as Abstract and Introduction, Literature Review, Model and Main Results, each technical-result section, Numerical Study, Conclusion, and E-Companion Proofs. Adapt names to the actual manuscript.
4. Within each pass, separate findings into Writing Quality, Technical Correctness, and Exposition. Writing Quality includes grammar, terminology, notation consistency, undefined notation or concepts, cross-reference style, caption-text mismatch, and informal phrasing.
5. For technical sections, check theorem/proposition statements against proof logic, assumptions, notation, boundary cases, constants, equations, algorithms, and examples. Record positive verifications only when the check was actually done.
6. For experiments, check that claims match implemented designs, baselines, tables, captions, parameter names, figures, and robustness results. Do not accept an introduction or abstract promise unless the experiment section supports it.
7. Run a global consistency sweep after section passes. Include notation consistency, terminology consistency, cross-reference and label consistency, capitalization of formal elements, citation-year or publication-status concerns, and table/figure naming consistency. Treat notation and terminology as manuscript-level contracts, not local style choices.
8. Reconcile duplicate findings, including any pre-read issues, with the section review.
9. Produce summary statistics by category and status. Exclude positive "Verified" technical checks from issue counts unless they required a fix.
10. End with low-confidence or author-decision items for coauthor review.

Record pending naming decisions under [terminology discipline](terminology-discipline.md), while completing independent checks and authorized edits.

## Verification Discipline

- Use IDs that encode location: `S1.01` for Section 1 issue 1, `S9.03` for E-Companion issue 3, and `G10.01` for global sweep issues.
- Use types: Grammar, Terminology, Technical, Exposition, Notation, Cross-reference, Citation, Table/Figure, Experiment.
- Use confidence levels: High for objective or directly verified issues, Medium for likely but context-sensitive issues, Low for author judgment or taste.
- Use statuses: Identified, Fixed, Deferred, Author Decision Needed, Verified, Clean, No action needed.
- Use `Author Decision Needed` for unresolved new names or substantive renames. Honor an explicit author decision already provided; a literature synonym alone does not require renaming.
- Reserve `Verified` for technical claims, proofs, algorithms, or references that were checked in substance.
- Reserve `Clean` for a completed sweep with no issue found.
- If the manuscript files are incomplete, say exactly which checks could not be guaranteed.
- When fixing text, preserve a log entry with the original problem, the fix, and the status. Do not replace the audit with a vague assurance.
- Use `Fixed` only after the edit was applied and checked. An accepted but unapplied suggestion remains a recommendation, with acceptance recorded separately.
- Use approximate line numbers only when stable exact line numbers are unavailable, and label them as approximate.

## Expected Output

Return either a claim-evidence audit table or a pre-submission review log.

For claim-evidence audit, include:

- Claim.
- Location.
- Supporting result or experiment.
- Status: supported, conditional, overstated, missing, or unclear.
- Required fix.

For a full pre-submission review, adapt [the report template](../assets/pre-submission-review-template.md), retaining inspected scope, located findings, verification status, and unresolved decisions. A useful structure is:

1. Pre-Submission Review Log header.
2. Review Structure and status definitions.
3. Pass-by-pass section audit with tables.
4. Global Consistency Sweep.
5. Issues Found During Initial Read, if a separate pre-read was used.
6. Summary Statistics.
7. Low-Confidence Items for Co-Author Review.

## Common Failure Modes

- Revising a paragraph locally while breaking the paper's global promise.
- Letting the introduction advertise an unimplemented numerical feature.
- Changing terminology between body and appendix.
- Changing notation between model, results, experiments, and appendix.
- Creating new terminology during polish when an established manuscript term already exists.
- Treating a literature synonym as permission to replace a formally defined manuscript term.
- Recording an unverified recollection as literature evidence for a term.
- Defining one concept twice under different names or one symbol twice for different objects.
- Forgetting assumptions in the abstract or managerial implications.
- Marking a proof as verified after only reading the theorem statement.
- Declaring manuscript-wide terminology clean without checking variants across the whole manuscript.
- Declaring manuscript-wide notation clean without checking equations, statements, proofs, tables, captions, and appendix.
- Treating grammar polish as a substitute for technical rigor.
- Counting "no issue found" entries as fixed issues.
- Forgetting the appendix or electronic companion when the main text relies on deferred proofs.
- Reporting guaranteed status without naming what was inspected.
- Relying on undefined notation or concepts to explain a claim.

## Optional Full Example

If the user asks for the author's pre-submission review style, load [the sample log](pre-submission-samples/pre-submission-review-log.md). Use it as a structural example, not as reusable findings or verification evidence.
