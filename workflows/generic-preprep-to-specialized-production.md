# APPROVED — Generic Preprep to Specialized Production

**Status:** APPROVED  
**Last updated:** 2026-08-22

## Objective

Use a low-context AI system to build reusable blank structure, then use a context-aware system and human review to turn that structure into a trustworthy project deliverable.

The key distinction is:

- **Preprep:** What reusable structure should exist before the exact project content is known?
- **Prep:** Given this project's authorized sources and constraints, how should that structure be used?
- **Production:** Create the deliverable candidate.
- **Validation:** Test the candidate before approval or publication.

A polished template is still only a template.

## Portable workflow

```text
Generic scaffold engine
    -> generic preprep packet
    -> context-aware prep system
    -> production candidate
    -> human and source validation
    -> approved final product
```

Tera AI may serve as an example generic scaffold engine, while ChatGPT may serve as an example of a more tailored prep system. These are replaceable implementations. The durable standard is the artifact, provenance, stage boundary, and review process—not one vendor interface.

## Responsibilities

### Human

- define the real objective, audience, privacy boundary, and acceptance criteria;
- decide which sources are authoritative;
- approve what context a provider may receive;
- resolve disputed or consequential content;
- verify accessibility and final readiness;
- authorize publication.

### Generic scaffold AI

- create neutral sections, placeholders, schemas, and checklists;
- expose missing decisions;
- avoid project-specific invention;
- mark its output as a generic scaffold.

### Context-aware AI

- apply only authorized project context;
- preserve source provenance and unresolved questions;
- create a candidate rather than approve its own work;
- return uncertain or conflicting fields for human resolution.

## Generic preprep packet

A useful packet may include:

1. disclaimer and reader-guideline shells;
2. blank chapter, lesson, scene, or storyboard structure;
3. content-advisory and citation placeholders;
4. AI-assistance disclosure placeholder;
5. semantic-role legend;
6. accessibility requirements;
7. metadata and provenance;
8. prep handoff questions;
9. validation and publishing checklist.

Use [`../templates/content-preprep-packet-template.md`](../templates/content-preprep-packet-template.md) as a public-safe starting point.

## Semantic roles before colors

For color-coded documents such as web novels, store meaning as a role:

```text
narration
dialogue
inner-thought
source-quotation
learning-note
system-note
content-advisory
```

Map each role to presentation later:

```text
semantic document
    -> light theme
    -> dark theme
    -> high-contrast theme
    -> print / monochrome
    -> EPUB
    -> plain text
```

Color must not be the only cue. Preserve document structure, labels or other non-color differentiation, contrast, and plain-text meaning.

## Privacy gate

Before sending anything to the generic scaffold system:

- remove confidential names, source text, private paths, credentials, unreleased material, and proprietary examples;
- replace necessary examples with neutral placeholders;
- provide only the minimum structural information required;
- check the provider's current data-handling terms when sensitive information could be involved.

A public derivative should teach the transferable method without requiring access to the private project that inspired it.

## Verification

Before prep:

- confirm the packet is marked `artifact_type: generic-scaffold` and `status: DRAFT`;
- confirm project-specific facts remain placeholders;
- confirm required sources and human decisions are listed;
- confirm semantic roles are independent from colors;
- confirm the artifact can leave the originating provider.

Before publication:

- verify every resolved field against an authorized source;
- review privacy, licensing, citations, and disclosure language;
- test accessibility and non-color fallbacks;
- record the human approval and final revision.

## Failure and recovery

- If the generic tool invents project content, remove it and return to preprep.
- If project sources conflict, pause prep and escalate the conflict; do not average them.
- If semantic meaning disappears without color, repair the document structure before rendering.
- If a provider cannot export a durable artifact, treat the output as disposable and copy only reviewed, non-sensitive structure into the portable packet.
- If validation fails, return the artifact to the earliest stage that can correct the cause.

## Capability evidence

A learner demonstrates this workflow when they can:

- explain the difference between preprep and prep;
- classify what information belongs in each stage;
- build a provider-portable generic packet;
- prevent private context from leaking into a generic or public artifact;
- design semantic roles that remain understandable without color;
- identify the required sources and validation gates for a real project.

AI-generated templates alone are not evidence that the learner can perform these judgments independently.

