# OR/MS Research Workflow

A Codex skill for theory-driven and analytically grounded operations management,
operations research, and Management Science-style papers. It supports reading,
research development, drafting, proof review, experiment design, and manuscript audits.

## Usage

Ask for the deliverable and supply the relevant evidence, for example:

- Use $or-ms-research-workflow to assess the feasibility of this model idea.
- Rewrite this theorem interpretation while preserving its assumptions and benchmark.
- Draft an introduction from these preliminary results and identify unresolved claims.
- Audit this manuscript's claims against its proofs and numerical evidence.

The skill follows the user's requested scope. A section edit stays local; a full
pre-submission audit produces an evidence-backed review log. Missing materials
limit the conclusions that can be verified, but do not prevent useful conditional work.

## Files and Workflows

- [SKILL.md](SKILL.md): shared research constraints, authorization boundaries, and output defaults.
- [manifest.yaml](manifest.yaml): route index for all research and writing modules, including abstracts.
- [references](references/): guidance loaded for the requested task.
- [assets](assets/): adaptable templates for structured deliverables.
- [AGENTS.md](AGENTS.md): repository maintenance instructions.
- [agents/openai.yaml](agents/openai.yaml): display metadata and default prompt.

Terminology follows manuscript definitions, then identifiable literature, then
neutral description. The [decision protocol](references/terminology-discipline.md)
covers new names, conflicts, and provenance audits. New names need author approval
before adoption; routine reuse of defined terms needs no separate approval.

Annotated introductions and review samples are available through their references.
They illustrate structure and style, not verified findings for a new manuscript.
