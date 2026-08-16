# Learning Debt

**Learning debt** is the gap between what a project required and what the learner can personally understand, explain, reproduce, adapt, diagnose, verify, prompt for, or teach.

It is not the same as project failure. A project can succeed while substantial learning debt remains.

## Why Track It

Without explicit tracking, AI-assisted productivity can hide dependency. Recording learning debt keeps that dependency visible so the learner can decide what deserves deeper study.

## Prioritize by Risk and Value

Not every gap requires immediate remediation. Prioritize learning debt when it affects:

- safety or security;
- money or legal obligations;
- architecture or production reliability;
- client or employer commitments;
- irreversible operations;
- the ability to detect important AI errors;
- recurring work the learner intends to own more independently.

## Example Record

```text
Capability required: Diagnose failed API authentication
Project result: Fixed with AI assistance
Learner can explain: Request/response flow and status code
Learner cannot yet reproduce: Token refresh debugging without guided steps
Learning debt: OAuth/token lifecycle diagnosis
Priority: High because this recurs in production work
Next action: Guided reproduction followed by reassessment
```

Learning debt should be treated as useful diagnostic information, not as a source of shame.
