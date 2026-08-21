# PROPOSED — Portable AI Memory Foundations

**Status:** PROPOSED  
**Track:** Human-Led AI Systems Literacy  
**Format:** Instructor-led lesson + Canva slide deck + guided lab  
**Suggested duration:** 90–120 minutes  
**Difficulty:** Beginner → Intermediate

## Lesson purpose

Teach learners how to design AI memory so that important knowledge remains portable across providers, tools, and machines instead of being trapped inside one chat platform.

The learner should understand that a useful memory system is not the same thing as storing every conversation. Durable memory requires separation between raw history, trusted knowledge, retrieval indexes, and task-specific context.

## Central idea

> **Own the memory; rent the intelligence.**

An AI provider may change, disappear, lose context, or use a different memory feature. Durable knowledge should therefore live in a provider-neutral form that can be versioned, inspected, backed up, and loaded into different AI environments.

## Learning outcomes

By the end of the lesson, the learner should be able to:

1. explain the difference between raw episodic history and curated semantic memory;
2. explain why Git can serve as durable memory authority without being the runtime search engine;
3. describe the four-layer portable-memory model;
4. identify provenance, status, authority, sensitivity, and supersession as memory-management concerns;
5. design a simple folder/schema model for a small AI-memory repository;
6. explain why embeddings/vector databases should be treated as rebuildable indexes rather than the only copy of memory;
7. construct a small context pack for one task instead of dumping an entire archive into an AI;
8. identify privacy and secret-management risks in conversation exports;
9. write an AI prompt that requests memory retrieval using subject knowledge rather than vague instructions;
10. teach the architecture back using a diagram or short presentation.

## Prerequisites

Learners should know:

- basic files and folders;
- what a Git repository is at a conceptual level;
- what an AI chat/context window is;
- the difference between private and public information.

Git command-line mastery is **not** required for the conceptual lesson.

## Key vocabulary

### Episodic memory
A record of what happened: conversations, events, sessions, timestamps, and chronological history.

### Semantic memory
Durable meaning extracted from experience: facts, definitions, rules, decisions, relationships, and stable knowledge.

### Procedural memory
Reusable instructions for how to perform a task.

### Provenance
Evidence showing where a memory came from.

### Authority
Who or what is allowed to establish a claim as trusted knowledge.

### Supersession
Preserving the history of a changed fact or rule by linking the newer record to what it replaces.

### Retrieval index
A search structure such as full-text search, embeddings, or a graph that helps find canonical memory but is not itself the permanent source of truth.

### Context pack
A bounded set of relevant memory supplied to an AI for one task.

## The four-layer model

```text
1. RAW EPISODIC VAULT
   conversations / exports / transcripts
              ↓
2. CURATED MEMORY AUTHORITY
   facts / decisions / workflows / project state
              ↓
3. REBUILDABLE RETRIEVAL INDEX
   full-text / vector / graph / cache
              ↓
4. CONTEXT PACK
   only the memory needed for this task
              ↓
             AI
```

### Layer 1 — Raw episodic vault

Stores history and evidence. It may contain provider exports, chat snapshots, timestamps, attachment references, and chronological sessions.

**Important:** history is not automatically truth.

### Layer 2 — Curated memory authority

Stores information that is expected to matter later and whose status can be understood.

Examples:

- approved project decisions;
- current project state;
- reusable procedures;
- known facts;
- stable preferences;
- lessons from failures;
- relationships among projects, people, systems, or decisions.

### Layer 3 — Rebuildable retrieval index

Makes memory fast to search.

Possible tools:

- Git-native search;
- SQLite/FTS;
- embeddings/vector databases;
- graph databases;
- generated manifests or summaries.

The key design rule is:

> If the retrieval database disappears, the durable memory should still exist and the index should be rebuildable.

### Layer 4 — Context pack

The AI receives the smallest useful memory set for the task.

A good context pack may include:

- the active project;
- relevant decisions;
- current constraints;
- one or two procedures;
- source provenance;
- unresolved conflicts;
- the user's newest instruction.

It should exclude unrelated history.

---

# Canva Teaching Storyboard

Use a 16:9 presentation. Keep one teaching idea per slide. Prefer diagrams, flow arrows, comparison cards, timelines, and simple repository trees over decorative stock imagery.

## Slide 1 — Title

**Portable AI Memory**  
*How to preserve knowledge when the AI platform changes*

Instructor prompt: ask, “If your favorite AI account disappeared tonight, what knowledge would you actually lose?”

## Slide 2 — The problem

Show three isolated AI platforms with separate memory bubbles.

Key message:

> Provider memory is convenient, but provider memory is not portable ownership.

## Slide 3 — Chat history is not enough

Two columns:

**Raw conversation**
- brainstorming
- corrections
- abandoned ideas
- timestamps
- duplicated statements

**Durable memory**
- accepted facts
- decisions
- procedures
- project state
- provenance

Ask learners which side should influence a future AI answer more strongly.

## Slide 4 — Episodic vs semantic memory

Use a simple example:

```text
Chat:
“I might use blue.”
“No, keep green.”

Semantic memory:
Approved color = green
```

Teaching point: extraction must preserve the difference between proposal and accepted truth.

## Slide 5 — The four-layer architecture

Use the main four-layer diagram.

Have learners name each layer aloud before continuing.

## Slide 6 — Why Git?

Show a Git repository with arrows for:

- version history;
- diff;
- rollback;
- branches;
- human review;
- plain text;
- backup/clone.

Teaching point: Git is excellent for **authority and history**.

## Slide 7 — What Git is not

Show a comparison:

**Git is good at**
- durable records
- history
- review
- portability

**Git alone is not ideal for**
- semantic nearest-neighbor search
- fast embedding lookup
- large-scale graph traversal
- token-budget optimization

Teaching point: do not force one tool to perform every layer.

## Slide 8 — Raw vault vs canonical brain

Draw two repositories:

```text
Private Raw Vault       Curated Knowledge Repo
full chats              trusted reusable knowledge
provider snapshots      decisions
session evidence        workflows
sensitive metadata      project state
```

Explain why raw transcripts deserve stronger privacy boundaries.

## Slide 9 — Memory needs provenance

Show a memory card:

```yaml
statement: Project uses PostgreSQL
status: APPROVED
source: architecture decision 004
captured: 2026-08-21
supersedes: SQLite prototype
```

Ask: “How is this stronger than a sentence copied from an old chat?”

## Slide 10 — Capture is not canon

Animate or reveal:

```text
CAPTURE
  ↓
CANDIDATE
  ↓
CLASSIFY
  ↓
CHECK CONFLICT / DUPLICATE / AUTHORITY / PRIVACY
  ↓
PROMOTE
```

Core phrase:

> The AI may extract a candidate. The extraction itself does not establish truth.

## Slide 11 — Supersession

Use a timeline:

```text
v1: Database = SQLite
        ↓ changed because multi-user requirement
v2: Database = PostgreSQL
```

Do not erase v1. Preserve why the decision changed.

## Slide 12 — Retrieval indexes are disposable

Show:

```text
Git memory → build index → search
```

Then delete the index visually and rebuild it.

Teaching point:

> Losing the index should be inconvenient, not catastrophic.

## Slide 13 — Context packs

Scenario:

“Fix authentication in Project Falcon.”

Load:
- Falcon architecture;
- auth decision;
- current error;
- relevant workflow.

Do not load:
- unrelated art project;
- old conversations about another app;
- entire chat archive.

## Slide 14 — Privacy boundary

Use four sensitivity cards:

- Public
- Internal
- Private
- Restricted

Emphasize that API keys, passwords, tokens, private keys, and other credentials should not become ordinary AI memory.

## Slide 15 — Guided lab

Give learners six statements from a fictional project and ask them to classify each as:

- raw episodic only;
- candidate memory;
- durable semantic memory;
- procedural memory;
- project memory;
- decision memory.

## Slide 16 — Failure case

Present a fictional AI that remembers:

> “The app uses Firebase.”

But the repository contains a newer approved decision:

> “PostgreSQL + custom auth replaced Firebase.”

Ask learners what the resolver should do.

Expected answer: prefer the authoritative current record, preserve the old record as superseded, and do not merge both into a false compromise.

## Slide 17 — Prompt from knowledge

Weak prompt:

> “Remember everything about my project and help me.”

Knowledge-based prompt:

> “Retrieve the current approved architecture, authentication decisions, active blockers, and relevant implementation workflow for Project Falcon. Exclude superseded decisions unless they explain the current state. Surface conflicts instead of guessing.”

Discuss why the second prompt is better.

## Slide 18 — Assessment bridge

Ask learners to design a memory architecture for one real project they already use.

Evidence should include:

- memory classes;
- raw/canonical separation;
- provenance plan;
- privacy boundary;
- retrieval strategy;
- one context-pack example.

## Slide 19 — Challenge bridge

After successful assessment, challenge the learner to implement a working minimum system:

```text
Git repository
+ normalized memory record
+ text retrieval
+ context-pack generator
```

Vector search is optional. The challenge is portability and correctness, not unnecessary technical complexity.

## Slide 20 — Teach-back

Learner must explain in three minutes:

1. why chat archives are not the same as trusted memory;
2. why Git can be the authority but not necessarily the runtime database;
3. why context packs matter;
4. why provenance and supersession matter.

End with:

> **Own the memory; rent the intelligence.**

---

# Guided Practice

## Practice A — Memory classification

Use this fictional project history:

1. “Maybe use MongoDB.”
2. “PostgreSQL selected because relational reporting is required.”
3. “Deployment failed because environment variable names differed.”
4. “Use the deployment checklist before production releases.”
5. “Version 1 shipped on August 10.”
6. “The learner prefers visual diagrams for architecture explanations.”

Learner classifies each item and explains whether it belongs only in raw history, in a candidate queue, or in durable memory.

## Practice B — Build one memory record

Create a provider-neutral record with at least:

```yaml
id:
type:
statement:
status:
source:
captured_at:
sensitivity:
supersedes:
relations:
```

The learner must explain what each field contributes.

## Practice C — Build a context pack

Task:

> “Prepare the next deployment for the fictional app.”

Learner chooses only the memories needed for the deployment task and explains exclusions.

---

# Verification Exercise

The learner should answer:

1. Can the durable memory be reconstructed without one specific AI provider?
2. Can the origin of an important claim be located?
3. Can a superseded fact be distinguished from a current one?
4. Can a raw chat statement remain untrusted until reviewed?
5. Can the search index be rebuilt from the durable source?
6. Can sensitive records be excluded from a provider context pack?

If any answer is “no,” the design still has portability or governance debt.

---

# Assessment Bridge

Use `[assessment]` only after guided practice.

A suitable authentic assessment is:

> Design the memory architecture for one real AI-assisted project. Produce a repository map, one normalized memory record, one supersession example, one privacy rule, and one task-specific context pack. Explain each design choice without relying on AI-generated wording as proof of understanding.

### Observable evidence

The learner can:

- distinguish archive from authority;
- justify the memory layers;
- identify unsafe or unnecessary retention;
- resolve a simple status conflict correctly;
- create a bounded context pack;
- explain how the system survives provider replacement.

### Learning debt to record

Possible untested areas:

- Git command-line implementation;
- vector database selection;
- automated secret scanning;
- embedding generation;
- production-scale ingestion;
- access-control implementation.

Do not mark these mastered merely because the conceptual architecture is understood.

---

# Challenge Bridge

After assessment evidence shows readiness, use `[challenge]` for a real implementation extension.

Suggested challenge:

> Build a minimal portable-memory prototype for a live project. Store durable memory in Git-tracked Markdown/JSON/YAML, implement exact-text retrieval with SQLite/FTS or equivalent, produce a context-pack generator, and demonstrate that deleting the runtime index does not destroy the canonical memory.

Required HLAPM challenge outputs should still include:

1. a learner-authored advanced implementation prompt;
2. a working live-project deliverable;
3. verification evidence;
4. a retrospective identifying AI assistance and remaining learning debt.

---

# Instructor Notes

## What not to teach

Do not reduce this lesson to:

> “Put your chats in GitHub.”

That teaches backup, not memory architecture.

The deeper lesson is separation of concerns:

```text
history ≠ truth
truth ≠ search index
search result ≠ context
AI output ≠ authority
```

## Public-example rule

Use fictional projects or sanitized examples. Do not publish real private conversation exports, credentials, private project canon, confidential customer information, or unreleased intellectual property.

## AI-assistance rule

AI may help the learner:

- understand vocabulary;
- compare designs;
- inspect sample schemas;
- critique a proposed architecture;
- generate practice data;
- identify missing verification questions.

The learner should personally demonstrate classification, architecture reasoning, context selection, conflict handling, and explain-back ability before mastery is claimed.

---

# Reuse Model

This lesson intentionally follows the reusable HLAPM lesson structure:

`Purpose → Outcomes → Vocabulary → Mental Model → Demonstration → Practice → Explain → Reproduce → Adapt/Diagnose → Verify → Prompt From Knowledge → Assess → Challenge → Teach → Record Learning Debt`

Future public lessons can use the companion `templates/lesson-model-template.md` to reproduce this teaching pattern in other technical and non-technical domains.
