# Storyline Analysis

## Purpose

Analyze whether an OM/OR paper has a clear, intriguing, and convincing storyline before the final rigor and consistency check. Focus on narrative logic, reader motivation, intellectual arc, insight clarity, section-to-section transitions, and Management Science positioning. Do not treat this as a grammar pass or proof audit, although story gaps may involve technical narrative issues.

## When to Use

Use before pre-submission rigor review, when the user asks whether the paper is compelling, convincing, attractive to readers, coherent as a story, or likely to hook an editor/referee at first glance.

## Inputs Needed

- Title, abstract, introduction, and contribution list.
- Section structure and main body text.
- Main results, experiments, and managerial implications.
- Target journal or audience.
- Closest benchmark papers or literatures when available.
- Any prior author comments about intended positioning.

## Core Distinction

Storyline analysis asks: "Will a reader understand why this paper matters, remember the main idea, and believe the journey from problem to insight to evidence?"

Rigor and consistency asks: "Are the claims, notation, proofs, experiments, references, and terminology correct and aligned?"

Keep these separate. In storyline analysis, flag technical issues only when they affect the narrative, such as a missing bridge between a theorem and an algorithm, an unexplained parameter, or an experiment whose role in the story is unclear.

## Procedure

1. Identify the big-picture story in one quoted paragraph. It should be memorable enough that a referee could repeat it.
2. Extract the narrative arc as a compact chain, such as `Practical Problem -> Structural Insight -> Algorithm -> Guarantee -> Experiments -> Managerial Meaning`.
3. Diagnose whether the paper has a strong first-glance hook. Check whether the abstract and introduction quickly reveal the decision problem, stakes, trade-off, and main insight.
4. Review section by section. For each section, state the narrative function, what works, and where the logical connection could be tighter.
5. Identify structural observations across sections. Look for multiple analytical "acts," missing bridges, delayed motivation, abrupt parameters, unsupported positioning, or experiments that feel detached from the theory.
6. Separate concerns into priorities. Use Priority 1 for gaps that weaken the main storyline, Priority 2 for technical-narrative depth, Priority 3 for audience positioning and exposition, and Priority 4 for optional refinements.
7. Produce an improvement plan with location-specific fixes. Each item should name the gap, the location, and the suggested fix.
8. If the user asks to implement fixes, add an implementation log after changes. Do not claim an item is done unless the manuscript was actually edited or the user explicitly accepted the revision.

## What to Check

- **Main idea memorability**: Can the story be summarized in one sentence without jargon?
- **Narrative arc**: Does each section naturally answer the question raised by the previous section?
- **Problem-to-insight bridge**: Does the paper explain why the central insight solves the stated problem?
- **Insight-to-method bridge**: Does the paper explain how the insight becomes a model, theorem, algorithm, experiment, or prescription?
- **Theory-to-practice bridge**: Does the paper explain what formal results mean for the decision maker?
- **Benchmark positioning**: Is the paper framed as a meaningful new question rather than a small extension?
- **Audience fit**: Does the paper lead with managerial and economic intuition before technical machinery when targeting Management Science?
- **Tension management**: If the paper has multiple analytical regimes, such as stochastic motivation and adversarial guarantee, are their roles explicitly distinguished?
- **Experiment role**: Do numerical or empirical sections validate the main principle, quantify value, explore mechanisms, or demonstrate robustness? Is that role stated clearly?
- **Ending power**: Does the conclusion reinforce the paper's remembered contribution rather than merely repeat the table of contents?

## Expected Output

Return a storyline analysis report with:

1. Big Picture Story.
2. Section-by-Section Analysis.
3. Structural Observations.
4. Improvement Plan.
5. Summary.
6. Implementation Log, only if fixes were actually made.

Use narrative paragraphs for diagnosis and tables for prioritized fixes. Mark whether each concern is about story logic, technical narrative, audience positioning, or exposition.

## Quality Bar

- Tie every criticism to a concrete section, transition, claim, parameter, result, or experiment.
- Distinguish "the story is weak" from "the claim is technically unsupported"; route the latter to rigor and consistency when needed.
- Prefer bridge-building fixes over vague advice. For example, propose a transition paragraph explaining why fluid analysis motivates an adversarially robust algorithm.
- Calibrate recommendations to the target journal. For Management Science, emphasize practical insight, decision relevance, mechanism, and credible evidence.
- Do not overfit the report to one paper's terminology. Preserve the reusable structure.

## Common Failure Modes

- Mistaking storyline analysis for proofreading.
- Producing generic comments such as "make the motivation stronger" without naming the missing logical bridge.
- Evaluating each section locally but failing to see the paper-level narrative arc.
- Letting the technical contribution overshadow the managerial question.
- Reporting an improvement as implemented when no manuscript edit was made.
- Ignoring the experiments' narrative role.
- Failing to explain why the central parameter, benchmark, or theorem should matter to readers.

## Optional Full Example

If the user asks for the author's storyline-analysis style, load `references/storyline-samples/storyline-analysis-report.md`. Use it as a report-architecture example, not as reusable findings.
