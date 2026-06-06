# Literature Reading

## Purpose

Read provided papers or notes as an OM/OR researcher by decomposing the paper rather than passively summarizing it. Identify how the paper abstracts reality into a model, how the model is solved, what trade-off generates the core insight, how the analysis is structurally assembled, and how the idea can migrate into new research questions.

## When to Use

Use when the user provides a paper, PDF text, abstract, introduction, notes, or citation context and asks what the paper says, why it matters, why it was publishable, or what can be learned.

## Inputs Needed

- Paper text, PDF extraction, abstract, introduction, or detailed notes.
- Target lens: writing, modeling, proof, experiments, positioning, or all.
- Journal or community if known.

## Procedure

Use a model-first pass before reading linearly.

1. **Model abstraction.** Ask what world the paper constructs. Identify variables, state/action spaces, decision maker, constraints, objective, information structure, timing, and uncertainty. Compress the paper into one optimization, equilibrium, stochastic-control, empirical, or design problem.
2. **Solution architecture.** Ask how the model is solved. Classify whether the paper uses closed-form first-order conditions, equilibrium characterization, dynamic programming, fluid/mean-field approximation, online algorithm, structural theorem, relaxation, numerical optimization, simulation, empirical identification, or pure numerical evidence. The goal is to know the solving route, not to reproduce every calculation.
3. **Core trade-off and insight.** Strip away context and state the central trade-off in one sentence. If the trade-off cannot be stated simply, the paper is not yet understood. Translate the main result into a mechanism: what force pushes one way, what force pushes the other way, and what changes the balance?
4. **Paper architecture.** Map how the paper is built. Locate the baseline, the changed assumption or added friction, the comparative statics, robustness checks, numerical experiments, extensions, and appendix proofs. Ask what each analysis is protecting against in reviewer terms.
5. **Extension and migration.** Ask how the trade-off can travel. Consider changing the setting, adding a key friction to a classic model, relaxing the least realistic assumption, changing the decision maker, changing the information structure, or connecting the model to a real operational constraint. Identify whether such changes could reverse, sharpen, or generalize the conclusion.

After the model-first pass:

6. State the paper's core research question.
7. Classify contribution type: new model, new setting, structural theorem, algorithm, empirical evidence, design prescription, robustness, or synthesis.
8. Explain why the paper could be publishable: importance, novelty, rigor, evidence, clarity, and positioning.
9. Distinguish what is borrowed, extended, and genuinely new.
10. Extract transferable writing or research-design lessons.
11. Do not infer unsupported claims from title, abstract, or reputation alone.

## Five Reading Questions

Ask these explicitly in a literature note:

1. **How does the paper model reality?** What variables, decision maker, constraints, objective, timing, and uncertainty compress the real setting into a formal problem?
2. **How does it solve the model?** What analytical or numerical route makes the result possible?
3. **What is the core trade-off?** What one-sentence mechanism remains after removing the application context?
4. **How is the paper structurally assembled?** What is the baseline, what assumption is changed, what comparative statics answer, and what robustness checks defend?
5. **How can the idea be extended?** Can the same trade-off move to a new industry, a classic model with one added friction, or a more realistic assumption?

## Expected Output

Use the literature note template when useful:

- One-sentence thesis.
- Model abstraction: variables, decision maker, objective, constraints.
- Solution architecture.
- Core trade-off and one-sentence insight.
- Paper structure: baseline, changed assumption, comparative statics, robustness.
- Extension and migration opportunities.
- Contribution logic.
- Key results and mechanism.
- Evidence or proof strategy.
- Why top-journal credible.
- Limitations and vulnerability.
- What to learn for the user's research.

## Common Failure Modes

- Summarizing section by section without identifying contribution logic.
- Reading introduction to conclusion without first extracting the model and trade-off.
- Describing the application context while missing the optimization problem beneath it.
- Listing results without explaining what trade-off creates them.
- Treating every technical novelty as a managerial contribution.
- Praising publishability vaguely.
- Inventing literature relationships not present in the text.
- Saying "this paper can be extended" without naming the transferable trade-off, new friction, or altered assumption.
