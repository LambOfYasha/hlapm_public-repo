# PROPOSED — Reconcile AI Memory with Human Review

**Status:** PROPOSED  
**Purpose:** Turn conflicting provider summaries into useful durable records and a separately reviewed public learning artifact.

Use this with [Portable AI Memory Foundations](../docs/lessons/portable-ai-memory-foundations.md) and [Session to Public Learning Artifact](session-to-public-learning-artifact.md). This workflow adds a practical reconciliation and publication-review procedure; it does not replace the memory architecture lesson.

## Outcome and responsibilities

The human decides which facts, preferences, roles, and proposed changes are accepted. AI can compare sources, draft records, identify conflicts, and prepare public teaching material. A prepared record does not establish truth, deployment, publication, or learner mastery.

The learner should be able to trace a claim to its source, distinguish a current decision from a historical experiment, justify exclusions, and verify exactly what a publication acceptance covers.

## 1. Establish the source and scope

Inventory the available sources with dates, versions, scope, and evidence type. A provider summary is a compressed account, not a transcript or proof of current operation. Check current project records rather than assuming the most verbose provider is correct.

A user may designate a preferred baseline. Use it as a conflict-resolution default while preserving contrary evidence and respecting newer explicit corrections. Do not merge contradictions into a compromise that no source supports.

Keep temporary project status separate from durable goals. A request to work on one item does not automatically reactivate all held work.

## 2. Classify each important claim

| Evidence or decision | Treatment |
|---|---|
| Explicit current human decision | Record within its stated scope and date |
| Approved current project record | Use as established context, subject to newer authorized changes |
| Assistant interpretation or recommendation | Preserve as proposed |
| Past experiment | Preserve as historical; do not infer a lasting preference |
| Tool or product preference | Record as changeable; verify installation/current use separately |
| Conflicting names or roles | Check identity, stage, version, alias and scope before renaming |
| Unsupported completion claim | Keep unverified until concrete evidence exists |
| Irrelevant personal or local-only material | Exclude from the destination |

Use fields such as statement, domain, source, source date, status, scope, supersedes, and last verified. Add story stage or implementation version only when relevant. Preserve unresolved questions without inventing values.

## 3. Use a decision register

Assign stable IDs to grouped questions. Present each claim, evidence, recommended disposition, and a place for the human's correction. Interpret agreement to a recommended treatment precisely: agreeing to retain an unverified publication claim does not verify that publication.

Apply subsequent corrections to both the main record and affected summaries. Preserve supersession history so old decisions remain understandable. Avoid making the reader choose between two contradictory current entries.

Separate stable shared context, task-specific context, sensitive context, and temporary status. An agent persona is a presentation role; it does not prove a deployed bot, independent authority, or a newly established fictional fact.

## 4. Prepare the public derivative privately

Classify each source item as PRIVATE, GENERALIZE, HOLD, or EXCLUDE. Convert useful methods into teaching material with generic examples. Do not publish private names, lore, exact source paths, personal information, unreleased intellectual property, or transcripts merely because the public artifact is educational.

Review all output surfaces: titles, file names, links, examples, metadata, diffs, commit messages, and PR descriptions. A draft PR or branch in a public repository is already public disclosure.

When there is no useful safe derivative, record NO PUBLIC DERIVATIVE. A conversion workflow does not require publication of every private update.

## 5. Request acceptance of the exact instance

Prepare a full draft or readable exact diff before asking. Include an instance ID and revision, intended target files, public benefit, omitted categories, checks, limitations, and hashes or exact artifact versions. Keep the source-to-derivative mapping private.

Use [the review template](../templates/public-conversion-review.md). Request acceptance, revision, or keeping the material private. State the exact action acceptance authorizes, such as creating a draft PR or committing selected files.

Do not treat a prior instance's acceptance, a general sync request, a schedule, silence, or permission to install a skill as acceptance of this version. Natural-language acceptance is sufficient when it clearly refers to the displayed packet; a magic phrase is unnecessary.

A material change to candidate content invalidates its earlier acceptance. Create a new revision and show the updated draft. If a repository baseline changes, compare it again and preserve unrelated work.

## 6. Apply and verify the accepted action

Write only the accepted files and action. For a draft-PR authorization, do not infer merge authorization. Record the resulting commit/PR and verification result. If blocked, retain the prepared packet and report the actual state.

Separate private-write status from public-publication status. A useful lifecycle is PREPARED → AWAITING HUMAN ACCEPTANCE → ACCEPTED → PUBLISHED, with REVISE, KEEP PRIVATE, NO PUBLIC DERIVATIVE and BLOCKED as explicit alternatives.

Avoid conversion loops: receipts, bookkeeping and unchanged mirrors do not create new learning by themselves.

## Worked example — fictional evidence

A fictional team has these records:

| Record | Reconciliation |
|---|---|
| Older summary: “We may choose Tool A” | Proposal, not selection |
| Later human decision: “Use Tool B for this prototype” | Scoped selection, not a permanent all-project rule |
| Summary: “The reporting bot is running” | Unverified without configuration or execution evidence |
| New request: “Correct the documentation while the project is paused” | Documentation-only exception |
| Public draft r1: “Learner mastery untested” | Matches available evidence |
| Public draft r2: “Learner has mastered the workflow” | Unsupported promotion; correct and obtain acceptance of the revised draft |

The useful public lesson is evidence-aware reconciliation, not the team's identity or private work. Generalization costs some narrative detail but preserves the reasoning readers can reuse.

## Practice, verification, and learning debt

Use a real documentation task with permission to inspect its sources. The learner classifies five claims, justifies one exclusion, resolves one contradiction, and prepares an exact review packet. AI may organize evidence and critique the draft. The learner owns the classifications, rationale, and explain-back.

Verify that:
- each promoted statement has an appropriate authority and scope;
- uncertain implementation remains unverified;
- private and public copies serve different purposes;
- examples remain accurate after generalization;
- the review identifies exact bytes or artifact versions and the intended action;
- no publication happened before acceptance.

Assessment evidence is the learner's explanation and demonstrated classification, revision, and verification. An AI-produced packet alone is not mastery. Record untested disclosure detection, tool operation, automation, or change-management skills as learning debt.

After demonstrated assessment readiness, an optional challenge is to manage two changed source versions through a real documentation release. Agree a fair deadline and acceptance criteria first; require a learner-authored advanced prompt, a finished deliverable, verification, and separate evaluation of knowledge, product quality, and deadline discipline.

Teach-back: explain in three minutes why a provider summary is not authority, why retention is not verification, and why an accepted revision cannot silently authorize different content.

