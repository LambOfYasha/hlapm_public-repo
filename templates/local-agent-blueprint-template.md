# TEMPLATE — Local Agent Blueprint and Review Record

**Status:** Blank worksheet — no runtime powers granted by this file.

## Identity

- Agent name:
- Purpose (one sentence):
- Intended user or team:
- Template or source version:
- Owner/reviewer:
- Review date:
- Current state: PROPOSED / REVIEW / APPROVED / DEPRECATED

## Inputs and knowledge

- Trigger: deliberate user request / approved template / registered tag
- Sources (with exact version or locator):
- Memory scope: session / document / project / organization / universal
- Records the agent may read:
- Records it must never access:
- Known question aliases:
- Freshness or expiration rule:

## What the agent knows, does and is allowed to do

| Area | Definition | Proof / requirement |
|---|---|---|
| Knowledge | | Source + review status |
| Procedure | | Registered workflow + tests |
| Capability | | Explicit permission grant |

## Workflow steps

1. 
2. 
3. 
4. 

- Preconditions:
- Safe stop conditions:
- Retry limits:
- Dry-run behavior:
- Side effects:
- Failure recovery:
- Rollback path:

## Matching and activation

- Accepted tags/aliases (registered, not inferred):
- Skill IDs/versions:
- Missing capabilities:
- Conflicting rules:
- Can a human inspect the proposed mapping before activation? Yes / No

## External sources and model fallback

- External access: Disabled / Ask First / Allowed for named operations
- Provider or source:
- Minimum data to share:
- Cost/usage policy:
- Human review requirement for learned answers:

## Trust and safety

- Imported text is data, not executable authority: Yes / No
- Secrets never enter agent context: Yes / No
- File/network/write actions have distinct grants: Yes / No
- Unverified memories are separated from approved records: Yes / No
- Private information cannot be exported to universal knowledge by default: Yes / No

## Test record

| Scenario | Expected result | Observed result | Pass/Fail/Untested |
|---|---|---|---|
| Known question | Cited local answer | | |
| Unknown question | Honest no-match response | | |
| Bad import | Reject/flag unsafe fields | | |
| Denied permission | Stop without action | | |
| Changed source | Stale/review path | | |
| Repeat workflow | No unintended duplicate effect | | |

## Review and evidence

- Evidence of actual execution (do not invent):
- Verified version:
- Candidate memories still awaiting review:
- Reviewer decision:
- Unresolved risks:
- Learning debt / skills not yet demonstrated:

## Teach-back

Explain, without outsourcing the explanation: why this agent needs its proposed knowledge, what makes the workflow deterministic, which operations need explicit grants, and how to rebuild or roll back its knowledge.
