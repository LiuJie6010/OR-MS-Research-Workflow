# Introduction Writing

## Purpose

Build a Management Science-style introduction that sells the research question to a busy editor while preserving the formal contribution. Use structured annotations as the collaboration layer between the human author and Codex: every paragraph should reveal its role, internal logic, big-picture function, and connection to the next paragraph before or beside the prose.

Treat introduction writing as a late-stage paper-writing module. The best introduction is usually written after the main body, formal results, numerical evidence, contribution list, and section roadmap are stable enough to reveal what the paper actually proves.

## When to Use

Use when drafting, revising, or critiquing an introduction, contribution block, abstract-adjacent overview, or paper roadmap.

If the body is not yet stable, return a conditional outline and a body-information checklist rather than pretending the final contribution storyline is known.

## Inputs Needed

- Real-world setting and decision maker.
- Decision objects or levers studied in the paper.
- Central trade-off with a grounded example.
- Closest prior work and restrictive assumptions.
- Research question.
- Main analytical answer and contribution list.
- Actual body-section structure for the roadmap.
- Any local style rules from the author, such as prohibited punctuation, emphasis commands, notation locks, or terminology locks.

## Procedure

Use this annotated narrative architecture:

1. Overall logic flow. Before drafting prose, write a compact map for P1 through the roadmap. Each line should state the paragraph role and the one-sentence content promise.
2. Design principles. Record the introduction-specific writing choices: what to lead with, what must stay visible, how the paper differs from the closest benchmark, how technical claims should be translated, and local style rules. Enforce definition-before-use: do not invoke formal notation, theorem labels, or technical concepts until they are defined in the manuscript or immediately defined in the same passage.
3. P1 Context. Open with the practitioner-facing setting. End by naming every decision object or lever the paper studies.
4. P2 Trade-off. Use one grounded example, preferably with numbers or concrete operational stakes, to show both extremes and why neither is enough. If the paper has multiple levers, show how each can forfeit the benefit when misaligned.
5. P3 Difficulty. Explain why the problem is hard on its own terms. Do not preview the answer here. Name uncertainty, non-stationarity, combinatorial explosion, coupling across decisions, information constraints, or computational barriers only when supported by the paper.
6. P4 Research question. Name the closest prior work, state what it assumes and proves, identify the restrictive assumption, and frame the paper as answering a different question when warranted. End with one clean research question.
7. P5 Managerial answer. Answer the research question at a plain-language level. Say what the paper means for practice before saying what it proves. Keep this block non-overlapping with the formal contribution list.
8. Contributions block. Use a numbered list with specific contribution verbs. Use four items when possible: model or representation, main structural theorem and robustness, optimization or prescription, numerical or empirical evidence. Add or remove items only when the body truly supports it.
9. Roadmap. Use one sentence per section and align labels with the actual manuscript.
10. Structure summary. After the draft, include a concise summary with paragraph roles, approximate lengths, the P5-versus-contributions split, and notation, terminology, or style locks.

## Annotation Protocol

When drafting or revising an introduction in LaTeX, use comments like the author's examples. Keep them concise enough to be useful but detailed enough that the human can inspect and redirect the logic.

For the header:

```tex
% =============================================================================
% OVERALL LOGIC FLOW
% P1 (Context):     ...
% P2 (Trade-off):   ...
% P3 (Difficulty):  ...
% P4 (Research Q):  ...
% P5 (Answer):      ...
% Contributions:    ...
% P6 (Roadmap):     ...
%
% DESIGN PRINCIPLES
% (a) ...
% (b) ...
% =============================================================================
```

For each paragraph:

```tex
% --- PARAGRAPH 2: TRADE-OFF ---
% Role: ...
% Internal Logic: ...
% Big Picture: ...
% Connection to Next: ...
```

For contribution items:

```tex
% --- CONTRIBUTION 2 ---
% Role: ...
% Selling points: ...
\item {\bf Precise contribution label.}
...
```

Use `Role` to state what job the paragraph performs, `Internal Logic` to list the sentence-level progression, `Big Picture` to explain why the paragraph matters for the editor, and `Connection to Next` when the transition is non-obvious. In contribution comments, use `Selling points` for body-supported formal claims, not aspirations.

## Expected Output

Return either a paragraph-by-paragraph outline or polished prose. Also provide a promise audit:

- Are all decision variables introduced early?
- Does P2 show the trade-off?
- Does P4 frame a new question instead of a small extension?
- Does P5 avoid duplicating the formal contributions?
- Does every contribution have support in the body?
- Does the roadmap match the manuscript's actual section labels and order?
- Does the draft preserve the manuscript's established notation and terminology?
- Do the annotations expose enough structure for a human coauthor to edit the logic without rewriting the prose from scratch?
- Does every symbol, theorem label, assumption, and technical concept appear only after it is defined or immediately defined in the same passage?

## Common Failure Modes

- Opening with technical definitions.
- Introducing a decision variable only in the contribution block.
- Saying "we extend" when the paper can be framed as a new research question.
- Previewing the answer before explaining the difficulty.
- Mixing the managerial answer and theorem-level contribution.
- Using contribution verbs such as "explore" or "discuss" when the paper proves or characterizes.
- Letting paragraph annotations become generic labels rather than a real logic map.
- Treating the closest paper as a small extension target when the introduction can frame a distinct research question.
- Letting P5 repeat theorem statements already reserved for the contribution block.
- Writing a roadmap from memory rather than from the actual body sections.
- Renaming a body construct or introducing a new label for a concept that already has an established manuscript term.
- Referencing formal notation, theorem labels, or concepts before they are defined.

## Optional Full Examples

If the user asks for imitation of the author's annotated introduction style, load one or both full LaTeX samples:

- `references/introduction-samples/annotated-dynamic-matching-introduction.tex`
- `references/introduction-samples/annotated-opaque-selling-introduction.tex`

Use these as structural examples, not as reusable prose. Preserve the user's annotation style: overall logic flow, design principles, paragraph-level comments, contribution-item comments, and final structure summary.
