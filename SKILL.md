---
name: or-ms-research-workflow
description: Research and paper-writing workflow for operations management, operations research, and Management Science-style papers. Use when Codex helps with OM/OR literature reading, research brainstorming, idea feasibility, model/proof rigor, theorem interpretation, Management Science prose, introduction/abstract/body writing, numerical experiment design, managerial insights, reviewer critique, revision audits, or consistency checks across claims, assumptions, proofs, experiments, and implications.
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
- Draft abstract, introduction, body, conclusion, appendix, or style revision: load `references/management-science-writing.md`; also load `references/introduction-writing.md` for introductions.
- Theorem, proposition, lemma, corollary, or proof text: load `references/theorem-interpretation.md` and `references/proof-rigor.md`.
- Numerical experiment plan, robustness checks, tables, or figures: load `references/experiment-design.md`.
- Managerial implication or post-result discussion: load `references/managerial-insights.md`.
- Whole manuscript critique: load `references/reviewer-critique.md` and `references/rigor-and-consistency.md`.
- Revision history, reviewer comments, co-author comments, diffs, or taste-memory updates: load `references/taste-evolution.md`.

When a task spans multiple modules, load the minimum set that covers the request. For example, a theorem interpretation rewrite should load management-science writing, theorem interpretation, and proof rigor.

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

Use templates in `assets/` when the user asks for a structured note, plan, outline, experiment plan, reviewer report, theorem interpretation, or revision audit.
