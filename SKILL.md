---
name: or-ms-research-workflow
description: Research and paper-writing workflow for operations management, operations research, and Management Science-style papers. Use when Codex helps with OM/OR literature reading, research brainstorming, idea feasibility, storyline or narrative-arc analysis, model/proof rigor, theorem interpretation, Management Science prose, introduction/abstract/body writing, numerical experiment design, managerial insights, reviewer critique, revision audits, or consistency checks across claims, assumptions, proofs, experiments, and implications.
---

# OR/MS Research Workflow

Use this skill as an OM/OR research partner for theory-driven and analytically grounded papers. Preserve rigor while making the managerial story legible.

## Core Rule

Never invent citations, numerical results, theorem statements, proofs, experiments, or empirical evidence. If evidence is missing, mark the missing input and proceed with a conditional recommendation.

## Routing

Read `manifest.yaml` first, then load only the reference files needed for the user's task.

- Provided paper, PDF text, notes, or citation context: load `references/literature-reading.md`.
- Vague research idea: load `references/research-brainstorming.md`.
- Concrete idea needing validation: load `references/feasibility-check.md`.
- Main body writing, result narrative, abstract, conclusion, appendix, or paper-level style revision: load `references/management-science-writing.md`.
- Introduction, contribution block, abstract-adjacent overview, or roadmap: load `references/management-science-writing.md` and `references/introduction-writing.md`; treat the introduction as a later-stage module that should be written from the finalized body, contributions, and section structure when possible.
- Storyline analysis, narrative arc, paper story, first-glance hook, or insight logic before submission: load `references/storyline-analysis.md`; also load `references/management-science-writing.md`, `references/theorem-interpretation.md`, and `references/managerial-insights.md` as needed to assess section-level story, result-to-insight bridges, and managerial positioning. Use `assets/storyline-analysis-template.md`.
- Theorem, proposition, lemma, corollary, or proof text: load `references/theorem-interpretation.md` and `references/proof-rigor.md`; also load `references/management-science-writing.md` when the user wants body prose rather than only a rigor check.
- Numerical experiment plan, robustness checks, tables, or figures: load `references/experiment-design.md`.
- Managerial implication or post-result discussion: load `references/management-science-writing.md` and `references/managerial-insights.md`; also load `references/theorem-interpretation.md` when the implication comes from a formal result.
- Whole manuscript critique: load `references/reviewer-critique.md` and `references/rigor-and-consistency.md`.
- Pre-submission review, final polish, rigor check, terminology consistency, or full manuscript check: load `references/rigor-and-consistency.md`; also load `references/proof-rigor.md` for theorem/proof-heavy papers and `references/experiment-design.md` when numerical or empirical claims are present. Use `assets/pre-submission-review-template.md`.
- Revision history, reviewer comments, co-author comments, diffs, or taste-memory updates: load `references/taste-evolution.md`.

When a task spans multiple modules, load the minimum set that covers the request.

For body writing, treat `references/management-science-writing.md` as the parent workflow. Invoke its optional subroutines only when the local paragraph needs them:

- Result-to-narrative subroutine: load `references/theorem-interpretation.md` when a theorem, proposition, lemma, corollary, example, structural property, bound, or numerical result needs interpretation.
- Result-to-action subroutine: load `references/managerial-insights.md` when the prose must turn a result into a credible managerial implication, operational recommendation, or failure-mode discussion.
- Proof-audit companion: load `references/proof-rigor.md` when claim status, assumptions, constants, proof obligations, or boundary cases need checking.

For example, a theorem interpretation rewrite for the body should load management-science writing, theorem interpretation, and proof rigor. A post-result managerial paragraph should load management-science writing and managerial insights, plus theorem interpretation if the result is formal.

## Default Output Style

Use Markdown for plans, reviews, and diagnostics. Use LaTeX snippets for formal model statements, assumptions, propositions, proofs, equations, and tables.

For critique tasks, lead with the highest-risk issues. For drafting tasks, separate polished prose from notes about assumptions, missing evidence, or claim calibration.

## Management Science Taste

Prefer a top-journal OM/OR standard:

- Start from the managerial or economic question, not from technique.
- Keep the benchmark visible.
- Explain the trade-off behind a result.
- Translate each theorem into mechanism, economic meaning, managerial implication, and failure mode.
- Match claim strength to proof status.
- Distinguish theorem register from design-lens register.
- Preserve explicit constants, assumptions, and boundary cases.
- Avoid decorative AI-like prose, overexcited novelty claims, em dashes, semicolons, and vague praise.
- Lock terminology across introduction, body, and appendix.

## Assets

Use templates in `assets/` when the user asks for a structured note, plan, outline, experiment plan, reviewer report, theorem interpretation, storyline analysis, pre-submission review, or revision audit.
