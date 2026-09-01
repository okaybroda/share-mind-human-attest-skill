# Share Mind Human Attest

A portable personal Agent Skill that asks the current participant in an AI-assisted work conversation to make the consequential judgments the agent cannot legitimately make.

It is designed to operate across domains without separate legal, software, medical, or financial prompts. It uses one policy: inspect the current artifact and available work trajectory, identify a consequential decision, and ask for the missing personal act of adoption, context, representation, tradeoff, accountability, dissent, escalation, or intervention.

## Why this exists

AI can produce complex work faster than a person can follow how it was made. The finished artifact may look polished while hiding consequential assumptions, tradeoffs, uncertainty, rejected alternatives, and decisions delegated to the agent.

Reviewing every generated step is often impractical, especially when the work is large, highly agentic, or high stakes. But letting those decisions disappear turns human oversight into a formality precisely where it matters most.

Share Mind identifies the consequential decisions that still require human judgment and brings them to the surface one at a time. It focuses on choices an AI cannot legitimately make for someone: which outcome to adopt, whose interests to represent, what risk to accept, who will take responsibility, and when to intervene, stop, or reverse course.

The goal is not to make the person reproduce the AI's work. It is to help them stay on top of it by making the important human decisions visible and explicit.

## What it does

- Runs explicitly with `$share-mind-human-attest` or, where supported, before an agent hands off work with evidence of high-stakes consequences.
- Inspects the current artifact and available trajectory.
- Asks one focused question at a time.
- Explains `Why this matters:` using the concrete stakes of the current work.
- Allows one focused follow-up for a missing response element.
- Rechecks work changed during questioning.
- Distinguishes completion, dissent, escalation, no-question inspection, and unresolved outcomes without treating dissent as failure.

It does not verify that the responder is human. It also does not verify identity, credentials, authority, unaided human authorship, correctness, safety, compliance, approval, exhaustive coverage, or a signature. It captures personal judgment, not organizational adoption, and does not replace professional review.

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

Automatic end-of-task activation is best effort and limited to work with visible evidence of genuinely high-stakes consequences because each harness controls skill discovery and invocation. Explicit invocation is the portable, reliable path for other work.

## Why conversation trajectory matters

The final artifact may hide assumptions, shortcuts, abandoned approaches, uncertainty, and decisions delegated to the agent. The visible trajectory helps locate those decisions. An earlier direct, explicit, change-specific decision from the participant may count when the work has not materially changed; generated summaries and inferred preferences never count. If context was compacted, the skill can disclose limited coverage and offer an optional deeper inspection of local session records when the harness makes them available.

## Project policies

- [Evaluation](EVALUATION.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)
- [Brand policy](BRAND.md)
- [Apache-2.0 license](LICENSE)
