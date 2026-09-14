# Maintaining OR/MS Research Workflow

These instructions apply to maintenance of this skill repository.

- Keep research behavior in [SKILL.md](SKILL.md), task-specific detail in references, and route metadata in [manifest.yaml](manifest.yaml). README describes usage; assets and samples are examples, not additional authority.
- Follow the user's requested scope and existing session authorization, subject to higher-priority instructions and tool permissions. Complete authorized local edits without repeated confirmation. This repository does not authorize publishing, sending messages, changing account settings, or modifying other installed skills.
- Preserve the skill's evidence standards, notation consistency, terminology provenance and author decisions. Do not turn a paper-specific convention into a general rule without supporting evidence.
- Keep route names and valid resource paths stable where possible. Update affected route metadata and documentation together; preserve unrelated user changes and invocation policy.
- For instruction edits, validate skill frontmatter, YAML, resource paths and the relevant behavioral boundaries. Run the available skill-creator validator and inspect the diff. Add broader checks only for a concrete unresolved concern; report checks actually performed and their limits.
- Model guidance informs prompt maintenance; it does not authorize API migrations, model-setting changes, mandatory delegation, or new approval gates.
