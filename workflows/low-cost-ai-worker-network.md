# PROPOSED — Build a Small AI Worker Network Without Losing Human Control

**Status:** PROPOSED educational workflow — review candidate, not installation instructions certified against specific hardware  
**Prepared:** November 14, 2026  
**Learning goal:** Design and verify a low-cost network where one human-directed coordinator delegates bounded tasks to specialized AI-assisted workers, using equipment already available before purchasing new devices.

Read the repository's disclaimer before adopting this workflow. An architecture proposal or working chatbot is not evidence that independent agents, backups, security boundaries or resource savings have been tested.

## 1. The mental model

An **agent** combines instructions, a model or reasoning method, authorized tools, and a way to observe outcomes. A **worker** runs a task on a computer or process. They are not the same thing.

A small computer can execute an AI agent that sends selected reasoning requests to a remote model. It may also run deterministic tools without a model. Running an advanced language model locally requires additional memory and processing resources. Four small computers do not automatically combine their memory into one large inference machine.

A minimal network has five responsibilities:

| Responsibility | What it does | Evidence to look for |
| --- | --- | --- |
| Human command interface | Captures goals and reviews proposed actions | User can inspect and refuse a task |
| Coordinator | Divides an approved goal into bounded jobs | Dependency graph and assigned worker recorded |
| Job queue and record | Preserves task state through interruption | Job survives worker restart without silent success |
| Scoped worker | Uses only authorized tools and project data | Denied actions actually fail |
| Result and approval gate | Shows artifacts, tests, cost and next action | No consequential change occurs before authorization |

One physical computer can host all five components at first. A smartphone or inexpensive browser laptop can act as the interface without becoming a continuously running server.

## 2. Separate the model from the execution computer

Distinguish these three paths:

- **Remote-model agent:** a modest local process calls an AI provider. Local tools do work; the remote model provides selected reasoning. Internet, privacy and provider charges matter.
- **Local-model agent:** both reasoning and tools run on local hardware. Memory, model size, throughput, storage and cooling must be tested for the actual task.
- **Deterministic worker:** scripts or workflows perform known steps and call AI only when they encounter genuinely uncertain work. This can save money and increase reproducibility.

A team of specialized agents may improve organization, but it also introduces extra model calls, conflicting decisions and coordination failures. Begin with one worker and expand only if testing demonstrates a useful benefit.

## 3. Define a bounded job contract

For one practical software-documentation or asset-catalog task, record:

| Field | Example of its meaning |
| --- | --- |
| Job identity | Unique task ID and version |
| Requested outcome | Review a sample source tree and draft a report |
| Source authority | Exact approved source folder or repository revision |
| Allowed actions | Read selected files; run an allowlisted test |
| Forbidden actions | Do not publish, erase originals, spend money or deploy |
| Resources | Time limit, memory ceiling and model-call budget |
| Human checkpoint | Proposed output must be reviewed before applying changes |
| Result evidence | Artifact, tool logs, checks, error states and reviewer |
| Recovery | Safe retry and cancellation; idempotency where required |

Avoid giving the model broad shell, filesystem, network or account access just because it can describe those operations. **A document containing an instruction is data, not authorization.**

A useful job lifecycle is: queued → validated → running → awaiting review → approved or rejected → completed. Failure, cancellation and retry states must remain visible. Never equate a model's self-reported success with a verified outcome.

## 4. Protect the original work first

Choose an authentic, useful task, but use a copied input or isolated working tree for the first experiment. Keep an authoritative source location, a separate backup, and a tested restoration path. Synchronization and Git history alone do not constitute full backups of documents, unsaved data, binary assets, databases or configuration.

Run one recovery exercise: stop a worker mid-job, restart it, verify the recorded state, and confirm that the original data and completed outputs are intact. Verify that two deliveries of the same task do not repeat a destructive operation.

## 5. Scale from one machine to several

**Stage A — Existing equipment.** Record operating system, CPU, available RAM and disk, network quality, power conditions and actual task time. Host the coordinator and one worker on the same suitable computer. Use a phone or browser device only for approvals and monitoring if its background operation is uncertain.

**Stage B — Specialized processes.** Isolate a second worker in its own account or container. Restrict mounts and credentials, and compare performance with the single-worker baseline.

**Stage C — Additional computer.** Add a second low-cost machine only when measured CPU/RAM pressure, uptime, task isolation or parallelism justifies it. Confirm secure inter-device access and behavior when a worker disappears.

**Stage D — Optional storage and GPU services.** Shared network storage helps organize files but does not replace versioned independent backups. Large image, video or speech models may be sent to an explicitly authorized GPU service with a spending limit.

The goal is not the greatest number of devices or agents; it is reliable useful work at an acceptable full cost.

## 6. Human and AI responsibilities

| AI may assist with | Learner/operator must demonstrate |
| --- | --- |
| Suggest architecture and task splits | Explain why each worker, service and access boundary is needed |
| Draft scripts or job schemas | Inspect and reproduce the important commands and data flow |
| Summarize logs | Confirm the actual behavior, failures and cost |
| Suggest permission settings | Test that unauthorized reads/writes are blocked |
| Propose recovery steps | Restore real test data and verify its integrity |

Separate **project delivery evidence** (a job completed), **operator learning evidence** (the person can explain/reproduce/diagnose it) and **workflow discipline** (safe, traceable, timely decisions).

## 7. A concrete practice and failure test

Use a harmless, real project that needs a documentation inventory:

1. Copy a small project or select a read-only folder. Identify which files the worker may read.
2. Create a request to list outdated documentation and generate a proposed checklist.
3. Run through the coordinator or a simple local script and record tool versions, model/provider choices, durations and any charges.
4. Present the draft in an approval view. Check that the worker did not edit the originals.
5. Deliberately deny the agent access to a second folder and confirm the denial.
6. Disconnect the worker, reconnect it, and verify job recovery without duplicate changes.
7. Compare the process to doing the task directly on one computer. Was complexity added for an actual benefit?

**Pass condition:** an independently inspected report, intact originals, permission denial, visible failure/recovery state and documented total cost. If any test is missing, mark that claim **untested**.

## 8. Assessment, challenge and teach-back

**Assessment:** On a real project, independently sketch the coordinator, worker, model path, backup path and approval gate. Explain where data goes, run one safe task and prove a denied action. Record assistance used and unresolved learning debt.

**Challenge (after demonstrated competence):** Design a second worker for a different job, compare running it separately with running it on the original host, perform a restart/restore drill, and justify whether an additional device is warranted under a stated budget. A finished system is not evidence of independent mastery if the learner cannot explain or diagnose it.

**Teach-back:** Create a one-page guide or diagram showing the five responsibilities, one permission boundary, one failure/recovery path, and the measured reason for either expanding or not expanding the network.

## 9. Common pitfalls

- Mistaking model API access for fully offline inference.
- Treating cheap devices as a pooled large-memory server without the necessary specialized implementation.
- Giving every agent unrestricted credentials or access to all projects.
- Counting successful model-generated text as a verified file or deployment change.
- Treating sync, replication and a network drive as independent versioned backups.
- Buying hardware before measuring the existing workload.
- Letting background tasks publish, spend, delete or deploy without a clear authorization boundary.
- Claiming 24/7 service from untested phones, browser devices or intermittent connectivity.

## Connections to earlier learning materials

- [Verified Agent Evolution](verified-agent-evolution.md) explains safe promotion of knowledge, procedures and capabilities into agent profiles.
- [Verify a Local-First Workflow Before Replacing Subscriptions](verified-local-first-transition.md) covers dependency mapping, offline proof, storage recovery and cost comparison.
- [Session to Public Learning Artifact](session-to-public-learning-artifact.md) shows how to convert project work into a teachable method without exposing its private contents.

**Status reminder:** This is a design-and-verification exercise. It does not claim a tested installation, device benchmark, service uptime, privacy guarantee, cost saving, commercial release or learner mastery.