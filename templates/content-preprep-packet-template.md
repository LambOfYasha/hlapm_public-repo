---
schema_version: 1
stage: preprep
artifact_type: generic-scaffold
status: DRAFT
provider: "[OPTIONAL_PROVIDER_AND_VERSION]"
created_at: "[DATE_OR_TIMESTAMP]"
project_context_applied: false
source_authority: none
structural_scope: template-only
requires_prep: true
requires_human_validation: true
---

# Generic Content Preprep Packet

> This is a reusable blank scaffold. It contains no project authority and is not ready for publication.

The YAML front matter above is the packet's machine-readable stage and provenance header. Implementations must parse and validate it before accepting the packet.

## 1. Intended use

- Deliverable type: `[WEB_NOVEL / LESSON / STORYBOARD / OTHER]`
- Intended audience category: `[AUDIENCE]`
- Required output formats: `[WEB / PRINT / EPUB / PLAIN_TEXT / OTHER]`
- Generic constraints: `[ACCESSIBILITY / LENGTH / STRUCTURE / OTHER]`
- Out of scope for this packet: `[PROJECT_FACTS / FINAL_WORDING / OTHER]`

## 2. Generic content disclaimer

### Fiction or creative-work notice

`[INSERT PROJECT-SPECIFIC WORDING DURING PREP]`

### Educational, professional, or source context

`[INSERT AUTHORIZED CONTEXT DURING PREP]`

### Content advisory

`[INSERT REVIEWED ADVISORY DURING PREP]`

### Sources and citations

`[INSERT SOURCE AND CITATION POLICY DURING PREP]`

### AI-assistance disclosure

`[INSERT ACCURATE PROJECT-SPECIFIC DISCLOSURE DURING PREP]`

## 3. Reader formatting guide

Explain how semantic content roles are communicated by structure, labels, typography, and optional color. Do not make color the only cue.

| Semantic role | Meaning | Non-color cue | Theme mapping |
|---|---|---|---|
| `narration` | `[DEFINE DURING PREP]` | `[HTML/DOCUMENT STRUCTURE]` | `[ASSIGN DURING THEME REVIEW]` |
| `dialogue` | `[DEFINE DURING PREP]` | `[LABEL/QUOTATION STRUCTURE]` | `[ASSIGN DURING THEME REVIEW]` |
| `inner-thought` | `[DEFINE DURING PREP]` | `[LABEL/TYPOGRAPHY]` | `[ASSIGN DURING THEME REVIEW]` |
| `source-quotation` | `[DEFINE DURING PREP]` | `[CITATION/BLOCK STRUCTURE]` | `[ASSIGN DURING THEME REVIEW]` |
| `learning-note` | `[DEFINE DURING PREP]` | `[LABEL/CALLOUT]` | `[ASSIGN DURING THEME REVIEW]` |
| `system-note` | `[DEFINE DURING PREP]` | `[LABEL/CALLOUT]` | `[ASSIGN DURING THEME REVIEW]` |
| `content-advisory` | `[DEFINE DURING PREP]` | `[LABEL/ICON/HEADING]` | `[ASSIGN DURING THEME REVIEW]` |

## 4. Blank content structure

Use portable labeled Markdown unless the target system defines and tests a richer syntax.

```markdown
# [TITLE]

## [SECTION OR CHAPTER]

### Block 001

- Semantic role: `narration`
- Speaker ID: `[NOT_APPLICABLE]`
- Source ID: `[NOT_APPLICABLE]`

> [CONTENT]

### Block 002

- Semantic role: `dialogue`
- Speaker ID: `[RESOLVE DURING PREP]`
- Source ID: `[NOT_APPLICABLE]`

> [CONTENT]

### Block 003

- Semantic role: `source-quotation`
- Speaker ID: `[NOT_APPLICABLE]`
- Source ID: `[RESOLVE DURING PREP]`

> [DO NOT INSERT SOURCE TEXT DURING PREPREP. RESOLVE DURING PREP AFTER SOURCE, PRIVACY, RIGHTS, AND CITATION REVIEW.]
```

## 5. Metadata placeholders

- Project ID: `[RESOLVE DURING PREP]`
- Content ID: `[RESOLVE DURING PREP]`
- Revision: `[REVISION]`
- Authorized sources: `[SOURCE_IDS]`
- Required reviewers: `[REVIEW ROLES]`
- Rights/licensing notes: `[REVIEW REQUIRED]`
- Accessibility target: `[STANDARD OR REQUIREMENTS]`
- Publication target: `[CHANNELS]`

## 6. Prep handoff questions

- What project and authorized source set applies?
- Which placeholders require a human decision?
- Which statements require citation or specialist review?
- Which semantic roles are actually needed?
- What private information may the tailored system access?
- What disclosure accurately describes the production process?
- Who may approve the final revision?

## 7. Validation checklist

- [ ] No invented project facts or citations
- [ ] Every factual or source-dependent field verified
- [ ] Privacy and confidential-source review complete
- [ ] Rights/licensing review complete where applicable
- [ ] Semantic roles preserved independently from color
- [ ] Contrast and non-color cues tested
- [ ] Plain-text/print fallback remains understandable
- [ ] AI disclosure matches actual use
- [ ] Required human reviewers approved the final revision
- [ ] Stage and provenance metadata updated

## 8. Known limitations and unresolved fields

`[LIST WITHOUT GUESSING]`

