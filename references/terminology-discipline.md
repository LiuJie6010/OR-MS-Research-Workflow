# Terminology Discipline

## Purpose

Govern technical terminology in OR/MS discussion and manuscript work so every named concept is traceable to the current manuscript, identifiable literature, or an explicit author decision. Do not apply this protocol to ordinary prose choices.

## Scope

Apply this protocol to technical constructs, model objects, mechanisms, regimes, policies, metrics, algorithms, acronyms, and named results. Treat terminology as distinct from notation, although both must remain consistent.

## Evidence Hierarchy

Use sources in this order:

1. **Current manuscript.** Preserve the term the author formally defines for the concept. Record the definition location when available.
2. **Identifiable literature.** If the manuscript has no term, use an established term only when a supplied or actually verified source supports that usage. Identify the source with a citation key, author and year, title, or precise location as available.
3. **Neutral description.** If neither source supplies an adequate term, describe the concept without giving it a new technical name.

Do not treat model familiarity, common-sounding wording, or an uncited recollection as evidence that a term is established. If literature support has not been checked, label the status as unverified rather than claiming standard usage.

When the manuscript and literature differ, keep the manuscript-defined term. Mention a literature synonym only when it materially improves positioning, searchability, or reader clarity, and state that the manuscript uses a different term. Do not silently rename the construct.

## Procedure

1. Search the manuscript, notes, definitions, tables, figures, captions, and appendix for the concept and its variants before drafting or recommending a change.
2. Record the manuscript term, definition location, variants, and whether the author has formally approved it.
3. If no manuscript term exists, check the literature materials supplied or sources actually verified for the task. Record the term and evidence rather than citing from memory.
4. Use the supported term consistently. Do not create stylistic synonyms for variety.
5. If no adequate supported term exists, continue with neutral descriptive wording.
6. If a new label would materially improve the manuscript, use `../assets/terminology-decision-template.md`. Keep the candidate only inside that decision note, explain why existing terms are insufficient, present alternatives, and request author approval.
7. While the decision is pending, do not use the candidate in discussion or manuscript prose as though it were established.
8. After approval, formally define the term in the manuscript before first use, record the decision and definition location, then treat it as a manuscript-defined term across the abstract, introduction, model, results, proofs, experiments, figures, tables, captions, conclusion, and appendix.

## Workflow-Specific Requirements

- In literature reading, distinguish the source's exact terminology from descriptive paraphrase.
- In brainstorming, use descriptive working language until the manuscript or literature supports a term; route any candidate name through the decision protocol.
- In abstracts and introductions, do not debut a technical term that is absent from the body and unsupported by literature.
- In theorem, proof, managerial, and experiment prose, preserve the manuscript's exact names for model objects, conditions, mechanisms, policies, metrics, and results.
- In reviews, flag unsupported, nonstandard, conflicting, or newly invented terms without silently replacing them.
- In skill maintenance, keep approved project terminology project-specific unless independent literature evidence supports a general rule.

## Expected Output

When terminology needs attention, report:

- the concept;
- the manuscript term and definition location, if any;
- the literature term and identifiable evidence, if any;
- conflicting variants or source mismatch;
- the wording used now;
- any author decision needed.

Use the terminology-decision template only when a new technical term is genuinely being proposed.

## Common Failure Modes

- Inventing a polished-sounding construct name during discussion and later treating it as established.
- Replacing an author-defined term with a literature synonym without discussion.
- Calling a term standard without identifiable evidence.
- Debuting an acronym or named mechanism in the abstract or introduction.
- Using synonyms for stylistic variety when they denote the same concept.
- Treating an approved project term as general OR/MS terminology.
