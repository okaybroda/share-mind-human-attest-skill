# Share Mind Human Attest

A portable Agent Skill that asks the person in an AI-assisted work conversation to make the consequential judgments the agent cannot legitimately make.

It works across domains because it does not encode separate legal, software, medical, or financial prompts. It uses one policy: inspect the current artifact and work trajectory, identify a material decision, and ask for the missing human act of adoption, context, representation, tradeoff, accountability, dissent, escalation, or intervention.

## Why this exists

AI can produce complex work faster than a person can follow how it was made. The finished artifact may look polished while hiding consequential assumptions, tradeoffs, uncertainty, rejected alternatives, and decisions delegated to the agent.

Reviewing every generated step is often impractical, especially when the work is large, highly agentic, or high stakes. But letting those decisions disappear turns human oversight into a formality precisely where it matters most.

Share Mind identifies the consequential decisions that still require human judgment and brings them to the surface one at a time. It focuses on choices an AI cannot legitimately make for someone: which outcome to adopt, whose interests to represent, what risk to accept, who will take responsibility, and when to intervene, stop, or reverse course.

The goal is not to make the person reproduce the AI's work. It is to help them stay on top of it by making the important human decisions visible and explicit.

## What it does

- Runs explicitly with `$share-mind-human-attest` or, where supported, before an agent hands off material work.
- Inspects the current artifact and available trajectory.
- Asks one focused question at a time.
- Allows one focused follow-up for a missing response element.
- Rechecks work changed during questioning.
- Ends with `Human judgment checkpoint complete` or `Human checkpoint incomplete` and explicit limitations.

It does not verify identity, credentials, unaided human authorship, correctness, safety, compliance, approval, exhaustive coverage, or a signature. It does not replace professional review.

## Install

Paste this into Codex or Claude Code:

```text
Install the Agent Skill from https://github.com/okaybroda/share-mind-human-attest-skill
```

## Use

Invoke it when the current work is ready for a decision checkpoint:

```text
Use $share-mind-human-attest on the work we just completed.
```

The skill asks in the active conversation. It does not post comments, create checks, or contact the hosted Socrates service.

Automatic end-of-task activation is best effort because each harness controls skill discovery and invocation. Explicit invocation is the portable, reliable path.

## Why conversation trajectory matters

The final artifact may hide assumptions, shortcuts, abandoned approaches, uncertainty, and decisions delegated to the agent. The available trajectory helps locate those decisions. It never counts as the participant's judgment; only a direct response after a checkpoint question can satisfy that question.

## Project policies

- [Evaluation](EVALUATION.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)
- [Brand policy](BRAND.md)
- [Apache-2.0 license](LICENSE)
