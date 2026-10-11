# PROPOSED — Verified Agent Evolution from Templates and Experience

**Status:** PROPOSED  
**Purpose:** Reusable, local-first method for turning manuals, templates, structured scripts, and verified troubleshooting into bounded agent capabilities.

## Principle

**Capture broadly; trust narrowly; execute only what was authorized.**

A useful agent evolution system distinguishes:

| Dimension | What changes? | Required control |
|---|---|---|
| Knowledge | FAQ, cited fact, terminology | provenance, scope, verification, freshness |
| Procedure | sequence of registered actions | validation, tests, version and rollback |
| Capability | permission to call an operation | explicit grant; never derived from source content |

## Entry points

- A user-written plan or blueprint
- A premade role or project template
- An approved manual or FAQ
- A registered tag/skill with typed parameters
- A captured demonstration of permitted application actions
- A reviewed solution to a recurring problem
- A connected external source or optional model suggestion

External data and AI outputs may supply **candidates**, not trusted instructions.

## Workflow

```text
Intake → classify & scope → parse explicit declarations
      → match existing role/skills
      → review conflicts and permissions
      → propose change (diff + sources)
      → test in safe mode
      → human approval
      → version and activate
      → measure results / rollback
```

### 1. Intake

Record the item's origin, version, owner, proposed scope, relevant files, and trust level. Do not execute imported code or a Markdown instruction during import.

### 2. Classify

Identify candidate facts, procedures, and capability requests separately. If the source is incomplete, mark what cannot be determined.

### 3. Match deterministically first

Use trusted manifests, registered tags, known aliases, and stable heuristics. Optional AI may *suggest* candidates, but must not silently modify the registry.

### 4. Inspect fit and conflicts

Show installed skills, missing skills, source references, requested commands, required grants, unknown fields, and contradictions with existing approved records.

### 5. Produce a reviewable proposal

Display exactly what will change. Separate knowledge approval from workflow installation and from a capability grant. Use the appropriate data scope.

### 6. Dry-run and test

Use safe fixtures. Test normal execution, missing source, malformed input, denied capability, interrupted execution, and repeated execution where side effects matter.

### 7. Approve, version, activate

Grant only necessary capabilities. Keep prior revisions for rollback and preserve the human decision and provenance.

### 8. Review results

Collect successes, failures, unanswered questions, and obsolete claims. Add repeatable findings to a candidate queue. Promote only after verification.

## Remote fallback policy

The agent should try verified local knowledge and approved workflows before considering a remote source. For a remote request, show the chosen provider, data to be shared, cost/privacy implications when relevant, and whether the user has authorized that class of access. Remote output returns as unverified evidence or a suggestion unless independently validated.

## Universal knowledge boundary

Promote only broadly reusable, reviewed methods. Do not propagate private workspaces, user histories, organization-specific rules, credentials, or unpublished materials into universal packs. The same restrictions apply to community contributions and exports.

## Failure and rollback

On ambiguous matching: show candidates, do not auto-enable. On missing permission: stop, do not escalate. On stale sources: warn or revalidate. On storage error: preserve the prior good state; no silent empty replacement. On a failed workflow: stop, report sanitized diagnostics, and revert reversible changes.

## Deliverable and evidence

A complete evolution record includes a source summary, change proposal, linked tests, capability diff, human review status, version, memory scope, and rollback plan. Learner mastery still requires observed explanation, reproduction and diagnosis; AI-generated artifacts are not sufficient evidence.

## Related resources

- [Agent Profile Blueprint Template](../templates/local-agent-blueprint-template.md)
- [Evolving Local Agents Without Model Dependence](../docs/lessons/evolving-local-agents-without-model-dependence.md)
- [Portable AI Memory Foundations](../docs/lessons/portable-ai-memory-foundations.md)
