---
name: or-ms-research-workflow
description: "Support OM/OR research and Management Science-style manuscripts: literature reading, idea feasibility, drafting, theorem interpretation, proof review, experiment design, terminology, and manuscript or revision audits. Use for research-content work, not generic document formatting."
---

# OR/MS Research Workflow

Help develop theory-driven and analytically grounded papers, connecting the managerial question to the model, evidence, and implications.

## Scope and Authorization

User instructions take precedence over this skill's workflow and style defaults, subject to higher-priority instructions and tool permissions. Infer the deliverable from the request and the session. Treat a request to draft, check, revise, or explain as the instruction to do that work, including phrasings such as "can you", "I want to", and "help me". Produce that result. Do not stop after acknowledging the task, proposing a plan, or offering to continue, and do not replace it with a narrower product.

Complete authorized work before asking, so a remaining question concerns a concrete result. Ask only when a missing answer materially affects correctness, scope, or authorization and cannot be reasonably inferred. State the assumption and continue the independent work. A narrow edit does not require a full-paper audit. Reference procedures and output outlines are defaults to adapt, not additional deliverables or approval gates. Input lists in references are useful evidence, not mandatory prerequisites. Do not add unsolicited approval steps, disclaimers, or hypothetical-risk checklists. Still label missing evidence and unresolved author decisions.

New technical terminology requires the author's approval before adoption. Existing explicit approval remains valid; do not request it again. Until approval, keep candidates in a separate decision note and use neutral wording in manuscript prose. Naming proposals do not block the rest of the task. The [terminology protocol](references/terminology-discipline.md) defines the evidence and decision record.

A research review or revision audit does not itself authorize editing this reusable skill, sending messages, submitting a manuscript, or publishing. Prepare the requested analysis or draft; perform external actions only within existing authorization. Do not delegate the requested work to subagents unless the user asks. If this skill causes a pause, an extra confirmation, unfinished requested work, or a change of direction, name and link the file that states the rule, quote the relevant text, distinguish an explicit requirement from an interpretation, explain what remains blocked, and complete unaffected work.

## Research Invariants

- Do not fabricate sources, results, proofs, experiments, or completed verification. Distinguish source claims, new derivations, conjectures, proposed experiments, and observed results. Label missing evidence and qualify conclusions.
- Match claim strength to evidence. Preserve material assumptions, quantifiers, explicit constants, thresholds, feasible sets, benchmarks, and boundary cases. A numerical example does not prove a universal claim.
- Preserve formally defined manuscript terms. If none exists, use terminology supported by identifiable literature; otherwise use neutral description. Familiarity alone is not evidence of established usage.
- Check affected definitions and uses before changing notation. One symbol denotes one object in its stated scope; one object has a consistent primary notation. Define new symbols and technical concepts before substantive use. A plain-language preview or resolvable forward reference to a later theorem is acceptable if understanding does not depend on undefined notation.
- Connect central results to mechanism, benchmark, and supported managerial meaning. Distinguish the limits of a guarantee from evidence that a conclusion fails outside its assumptions. Technical lemmas need not each yield a managerial recommendation.

## Routing

Use [manifest.yaml](manifest.yaml) as the route index. Select by the requested deliverable, not isolated keywords. Read the selected route's references; add conditional companions or subroutines only when their stated condition applies. A supplied paper is an input, not automatically a request for a literature review.

The terminology evidence hierarchy applies throughout. Load its detailed protocol for naming or renaming, conflicting or unsupported usage, provenance questions, or a terminology audit; routine reuse of a defined term does not require a separate ledger.

Templates under `assets/` are optional structures. Adapt them to the requested scope and format; omit irrelevant sections. Load full samples only for requested style imitation or a specific structural example, and never reuse their findings or numerical claims as evidence.

## Output and Verification

Follow the requested language and format. Otherwise use concise prose, Markdown for parallel diagnostic findings, and LaTeX for formal content. State the main point first, then the support it needs. Use a list when items are parallel, sequential, or easier to compare. Lead critiques with consequential findings. Deliver polished writing separately from material evidence gaps or author decisions. Avoid empty checklists, generic praise, decorative novelty claims, stock summary labels, and a contrast the user did not request.

Review the changed claims and their affected dependencies. A full manuscript audit retains the section-level evidence log described in [rigor and consistency](references/rigor-and-consistency.md). Report what was inspected and what remains unverified. Once the requested checks pass, stop. Repeat or widen them only when a new change, failure, or unresolved risk justifies it.
