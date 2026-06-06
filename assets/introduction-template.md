# Introduction Template

Use this lightweight structure when drafting a Management Science-style introduction with human-readable annotations. Prefer using it after the body, formal results, numerical evidence, contribution list, and roadmap are stable enough to reveal the paper's actual promise.

```tex
\section{Introduction}
\label{sec:intro}

% =============================================================================
% OVERALL LOGIC FLOW
% P1 (Context):     [Domain, practitioner setting, and decision objects/levers.]
% P2 (Trade-off):   [Core tension with a concrete example and both failure modes.]
% P3 (Difficulty):  [Why the problem is hard before revealing the answer.]
% P4 (Research Q):  [Closest benchmark, restrictive assumptions, and new question.]
% P5 (Answer):      [Managerial answer and main practical implication.]
% Contributions:    [Numbered items: model, theory, prescription, evidence.]
% P6 (Roadmap):     [Section-by-section outline matching the manuscript.]
%
% DESIGN PRINCIPLES
% (a) Lead with [realistic regime / managerial setting], not [technical baseline].
% (b) Keep [main decision objects/levers] visible throughout.
% (c) Frame the paper as [new research question], not only an extension of [benchmark].
% (d) Translate each structural result into managerial meaning before formal claims.
% (e) Local style rules: [terminology locks, punctuation, citation style, emphasis rules].
% =============================================================================

% --- PARAGRAPH 1: CONTEXT ---
% Role: Hook the reader with the real-world setting and introduce all decision objects.
% Internal Logic: [Broad setting] -> [specific applications] -> [why current practice creates the decision problem] -> [name the levers].
% Big Picture: Establishes why the problem is managerially important and what the paper studies.
[P1 prose.]

% --- PARAGRAPH 2: TRADE-OFF ---
% Role: Articulate the core tension through a concrete example.
% Internal Logic: [One side] -> [other side] -> [why each extreme fails] -> [why joint choice matters].
% Big Picture: Shows why the problem is not solved by a simple rule or single lever.
% Connection to Next: Sets up why the trade-off is technically hard to manage.
[P2 prose.]

% --- PARAGRAPH 3: DIFFICULTY ---
% Role: Explain why the problem is hard on its own terms.
% Internal Logic: [Uncertainty/non-stationarity] -> [combinatorial or analytical barrier] -> [coupling across decisions] -> [need for structure].
% Big Picture: Justifies a new framework instead of a routine optimization exercise.
[P3 prose.]

% --- PARAGRAPH 4: THE GAP AND RESEARCH QUESTION ---
% Role: Identify the closest benchmark and state the new question.
% Internal Logic: [Closest work] -> [what it proves] -> [restrictive assumptions] -> [why those assumptions bind] -> [research question].
% Big Picture: Frames the paper as answering a distinct question.
[P4 prose.]

% --- PARAGRAPH 5: OUR ANSWER ---
% Role: Answer the research question at a managerial level without duplicating the contributions.
% Internal Logic: [Name the core object/principle] -> [why it works] -> [what it implies for decisions] -> [point to formal contributions].
% Big Picture: Tells the reader what the paper means before listing what it proves.
[P5 prose.]

\subsection*{Our Contributions}

\begin{enumerate}
    % --- CONTRIBUTION 1 ---
    % Role: Establish the modeling or representation contribution.
    % Selling points: [Scope, decision objects, generality, benchmark contrast.]
    \item {\bf [Model or representation].}
    [Contribution prose.]

    % --- CONTRIBUTION 2 ---
    % Role: State the main structural theory and robustness.
    % Selling points: [Theorem, condition, guarantee, mechanism, robustness boundary.]
    \item {\bf [Structural theory and robustness].}
    [Contribution prose.]

    % --- CONTRIBUTION 3 ---
    % Role: Translate the theory into optimization or prescription.
    % Selling points: [Policy/design rule, decomposition, computability, managerial action.]
    \item {\bf [Optimization or prescription].}
    [Contribution prose.]

    % --- CONTRIBUTION 4 ---
    % Role: Validate practical relevance with numerical or empirical evidence.
    % Selling points: [Data/instances, baselines, metrics, robust pattern, limits.]
    \item {\bf [Numerical or empirical evidence].}
    [Contribution prose.]
\end{enumerate}

% --- PARAGRAPH 6: ROADMAP ---
% Role: Orient the reader to the paper's actual structure.
% Internal Logic: One sentence per section, in manuscript order.
% Big Picture: Keeps the introduction aligned with the body.
[Roadmap prose.]

% =============================================================================
% INTRODUCTION STRUCTURE SUMMARY
% Paragraph       | Role                                      | Approx. words
% P1 (Context)    | [Role]                                    | [...]
% P2 (Trade-off)  | [Role]                                    | [...]
% P3 (Difficulty) | [Role]                                    | [...]
% P4 (Research Q) | [Role]                                    | [...]
% P5 (Answer)     | [Role]                                    | [...]
% Contributions   | [Formal claims supported by body]         | [...]
% P6 (Roadmap)    | [Body alignment]                          | [...]
%
% Role split: P5 gives the managerial answer. The Contributions block carries
% precise formal claims and evidence. Avoid duplication between them.
%
% Style check: [terminology locks and local style rules].
% =============================================================================
```
