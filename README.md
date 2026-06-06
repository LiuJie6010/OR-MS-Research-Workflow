# OR/MS Research Workflow

This skill turns Codex into a focused research partner for operations
management, operations research, and Management Science-style paper work. It is
designed for theory-driven and analytically grounded projects where the hard
part is not only writing clearly, but keeping the research question, model,
proofs, experiments, and managerial implications aligned.

## What This Skill Is For

Use this skill when working on:

- OM/OR literature reading and paper taste extraction.
- Research idea brainstorming and feasibility checks.
- Management Science-style main body sections, result narratives, conclusions,
  appendices, abstracts, and paper-level style calibration.
- Late-stage introductions, contribution blocks, and roadmaps once the body
  clarifies the paper's real contribution.
- Theorem, proposition, lemma, corollary, and proof interpretation as body-writing
  subroutines when formal results need narrative meaning.
- Proof rigor checks, claim-proof alignment, constants, assumptions, and boundary
  cases.
- Numerical experiment design, robustness checks, figure planning, and table
  narratives.
- Managerial insight writing as a body-writing subroutine after formal or
  numerical results.
- Reviewer-style critique, pre-submission audits, revision planning, and
  consistency checks across a whole manuscript.
- Durable taste updates from co-author comments, reviewer comments, diffs, or
  repeated writing revisions.

The skill's central rule is simple: do not invent citations, results, theorem
statements, proofs, experiments, or evidence. If something is missing, the skill
should mark it explicitly and give conditional recommendations.

## How The Skill Works

`SKILL.md` provides the core workflow and routing rule. The agent first reads
`manifest.yaml`, then loads only the reference files needed for the user's
specific task. This keeps the working context focused instead of loading every
research guide at once.

The top-level taste standard is a top-journal OM/OR register:

- Start from the managerial or economic question, not from the technique.
- Keep the benchmark visible.
- Explain the trade-off behind each result.
- Translate theorems into mechanism, economic meaning, managerial implication,
  and failure mode.
- Match claim strength to proof status.
- Preserve constants, assumptions, thresholds, feasible sets, and boundary cases.
- Avoid decorative AI-like prose, vague novelty claims, and unsupported
  managerial statements.
- Keep terminology consistent across the introduction, model, results,
  appendix, figures, and conclusion.

## Workflow Structure

The writing workflow is intentionally hierarchical. `management-science-writing`
is the parent workflow for main-body paper writing. It can call
`theorem-interpretation` when a result needs mechanism, economic meaning, and
failure mode, and it can call `managerial-insights` when a result needs a
credible operational implication. Those files remain separate because their
paragraph structures are specialized, but they are not competing writing modes.

`introduction-writing` remains separate because introductions are best drafted
after the main body has stabilized: only then are the contribution list, formal
claims, evidence, and roadmap clear enough to write honestly.

## Modules

| Module | Use It For | Main Output |
| --- | --- | --- |
| `literature-reading` | Reading papers, abstracts, notes, or PDF text | Model-first paper decomposition with abstraction, solution route, trade-off, architecture, extensions, publishability, and lessons |
| `research-brainstorming` | Turning vague ideas into concrete research directions | Candidate research questions, mechanisms, minimum models, risks, and next checks |
| `feasibility-check` | Testing whether a concrete idea can become a paper | Feasibility memo with minimum viable paper, proof path, experiment path, and recommendation |
| `management-science-writing` | Parent workflow for main body text, result narratives, conclusions, appendices, and abstracts after the body is clear | Polished prose plus claim calibration, subroutine use, and style-risk notes |
| `introduction-writing` | Late-stage introductions, contribution blocks, and roadmaps | Paragraph architecture, polished intro prose, and promise audit |
| `storyline-analysis` | Pre-submission story, narrative arc, hook, and insight-logic review | Big-picture story, section-by-section storyline diagnosis, structural observations, and prioritized improvement plan |
| `theorem-and-proof` | Interpreting formal results and checking proofs, usually as a body-writing subroutine | Calibrated interpretation, rigor findings, proof obligations, and formal-status advice |
| `experiment-design` | Planning simulations, numerical studies, robustness checks, figures, and tables | Experiment questions, baselines, metrics, instance design, and narrative role |
| `managerial-insights` | Writing post-result implications, usually as a body-writing subroutine | Evidence-tied managerial paragraphs with mechanism and failure mode |
| `reviewer-critique` | Critiquing a section or full manuscript | Reviewer report with major concerns, rigor issues, managerial relevance, and revision priorities |
| `pre-submission-review` | Final full-manuscript audit before submission | Section-by-section review log for grammar, terminology, technical rigor, exposition, and global consistency |
| `revision-audit` | Learning from comments, diffs, revisions, or taste notes | Durable taste rules and suggested module updates |

## Templates

The `assets/` folder provides reusable output structures:

- `literature-note-template.md`
- `research-plan-template.md`
- `introduction-template.md`
- `storyline-analysis-template.md`
- `theorem-interpretation-template.md`
- `experiment-plan-template.md`
- `pre-submission-review-template.md`
- `reviewer-report-template.md`
- `revision-audit-template.md`

These templates are useful when the user asks for a structured note, research
plan, experiment plan, reviewer report, theorem interpretation, introduction,
storyline analysis, pre-submission review, or revision audit.

The introduction workflow also includes annotated full examples in
`references/introduction-samples/`. Load those samples only when the user asks
to imitate the author's annotated introduction style or when the introduction
logic needs a concrete structural model. Use them as annotation and architecture
examples, not as reusable prose.

The pre-submission workflow includes a full sample report in
`references/pre-submission-samples/`. Load it only when the user asks for the
author's pre-submission review style or when the audit report structure needs a
concrete model. Use it as a report-architecture example, not as reusable
findings.

The storyline workflow includes a full sample report in
`references/storyline-samples/`. Load it only when the user asks for the
author's storyline-analysis style or when the story report structure needs a
concrete model. Use it as a narrative-architecture example, not as reusable
findings.

## Example Prompts

```text
Use $or-ms-research-workflow to assess whether this model idea can become a
Management Science paper.
```

```text
Use $or-ms-research-workflow to rewrite this theorem interpretation so it
explains the mechanism, managerial meaning, and failure mode.
```

```text
Use $or-ms-research-workflow to design the numerical experiment section for this
theory paper.
```

```text
Use $or-ms-research-workflow to critique this introduction as a strict OM/OR
reviewer.
```

```text
Use $or-ms-research-workflow to analyze whether this paper's storyline is clear,
intriguing, and convincing before pre-submission review.
```

```text
Use $or-ms-research-workflow to audit whether the abstract, introduction,
theorems, experiments, and managerial implications make consistent claims.
```

## Repository Structure

```text
.
|-- SKILL.md
|-- manifest.yaml
|-- agents/
|   `-- openai.yaml
|-- references/
|   |-- experiment-design.md
|   |-- feasibility-check.md
|   |-- introduction-writing.md
|   |-- literature-reading.md
|   |-- management-science-writing.md
|   |-- managerial-insights.md
|   |-- proof-rigor.md
|   |-- research-brainstorming.md
|   |-- reviewer-critique.md
|   |-- rigor-and-consistency.md
|   |-- storyline-analysis.md
|   |-- taste-evolution.md
|   |-- theorem-interpretation.md
|   |-- introduction-samples/
|   |   |-- annotated-dynamic-matching-introduction.tex
|   |   `-- annotated-opaque-selling-introduction.tex
|   |-- pre-submission-samples/
|   |   `-- pre-submission-review-log.md
|   `-- storyline-samples/
|       `-- storyline-analysis-report.md
`-- assets/
    |-- experiment-plan-template.md
    |-- introduction-template.md
    |-- literature-note-template.md
    |-- pre-submission-review-template.md
    |-- research-plan-template.md
    |-- reviewer-report-template.md
    |-- revision-audit-template.md
    |-- storyline-analysis-template.md
    `-- theorem-interpretation-template.md
```

## Maintenance Notes

When improving the skill, keep `SKILL.md` lean and put detailed workflow guidance
in `references/`. Update `manifest.yaml` whenever a new reference module or
template should be routable. Use `taste-evolution.md` for durable lessons from
real revisions, but avoid overfitting the general skill to one paper, one
co-author, or one reviewer.

Before changing a module, ask whether the update captures a repeatable research
principle: contribution framing, proof rigor, claim calibration,
theorem-to-insight translation, experiment credibility, or managerial relevance.
Keep project-specific terminology in the project, not in the general skill.
