# HLAPM Lessons

This directory contains complete public teaching modules designed to move learners from explanation into observable capability.

A full HLAPM lesson should normally include:

1. **Purpose and learner outcome** — what capability the lesson is intended to build.
2. **Prerequisites** — what the learner should already know or have available.
3. **Core vocabulary** — terms the learner must be able to explain rather than merely repeat.
4. **Concept model** — a simple mental model before implementation detail.
5. **Guided demonstration** — a visible example with assumptions, verification, and AI/human responsibilities exposed.
6. **Practice** — a small learner-owned task.
7. **Explain-back** — the learner explains the concept in their own words.
8. **Reproduction** — the learner performs the process again with reduced assistance.
9. **Adaptation and diagnosis** — change one constraint and troubleshoot a failure.
10. **Verification** — show how correctness, provenance, privacy, or other relevant claims are checked.
11. **Prompt-from-knowledge exercise** — the learner writes a better prompt from acquired subject knowledge.
12. **Assessment bridge** — identify what could be demonstrated through authentic project work.
13. **Challenge bridge** — identify a harder real-project extension after assessment evidence exists.
14. **Teaching artifact** — slide deck, handout, diagram, demo, or other material that helps the learner teach the concept onward.
15. **Learning debt** — explicitly record what remains untested or dependent on AI.

## Canva-ready lessons

A Canva-ready lesson should include a slide storyboard with one teaching purpose per slide. Visuals should clarify system relationships, process, comparison, or evidence rather than merely decorate the deck.

Recommended deck rhythm:

`Problem → Mental Model → Vocabulary → Architecture → Walkthrough → Learner Practice → Failure Case → Verification → Assessment → Challenge → Teach-Back`

## Seed lesson

- [`portable-ai-memory-foundations.md`](portable-ai-memory-foundations.md) — teaches provider-independent AI memory using Git as durable authority, raw episodic capture, curated semantic memory, rebuildable retrieval indexes, and context packs.

## Reusable model

Use [`../../templates/lesson-model-template.md`](../../templates/lesson-model-template.md) when creating future HLAPM lessons.
