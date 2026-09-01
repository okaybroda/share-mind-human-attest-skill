# Share Mind Human Attest

A portable Agent Skill that asks the person in an AI-assisted work conversation to make the consequential judgments the agent cannot legitimately make.

It works across domains because it does not encode separate legal, software, medical, or financial prompts. It uses one policy: inspect the current artifact and work trajectory, identify a material decision, and ask for the missing human act of adoption, context, representation, tradeoff, accountability, dissent, escalation, or intervention.

## What it does

- Runs explicitly with `$share-mind-human-attest` or, where supported, before an agent hands off material work.
- Inspects the current artifact and available trajectory.
- Asks one focused question at a time.
- Allows one focused follow-up for a missing response element.
- Rechecks work changed during questioning.
- Ends with `Human checkpoint complete` or `Human checkpoint incomplete` and explicit limitations.

It does not verify identity, credentials, unaided human authorship, correctness, safety, compliance, approval, exhaustive coverage, or a signature. It does not replace professional review.

## Install

The repository root is a standard Agent Skills directory. Clone or copy it unchanged into a skills directory supported by your harness.

Codex user installation:

```sh
git clone https://github.com/okaybroda/share-mind-human-attest-skill.git ~/.codex/skills/share-mind-human-attest
```

Claude Code user installation:

```sh
git clone https://github.com/okaybroda/share-mind-human-attest-skill.git ~/.claude/skills/share-mind-human-attest
```

For another Agent Skills-compatible harness, use that product's documented skill directory or installer. The runtime skill has no provider, MCP, network, GitHub, or executable-script dependency.

## Use

Invoke it when the current work is ready for a decision checkpoint:

```text
Use $share-mind-human-attest on the work we just completed.
```

The skill asks in the active conversation. It does not post comments, create checks, or contact the hosted Socrates service.

Automatic end-of-task activation is best effort because each harness controls skill discovery and invocation. Explicit invocation is the portable, reliable path.

## Why conversation trajectory matters

The final artifact may hide assumptions, shortcuts, abandoned approaches, uncertainty, and decisions delegated to the agent. The available trajectory helps locate those decisions. It never counts as the participant's judgment; only a direct response after a checkpoint question can satisfy that question.

## Relationship to Socrates

This skill provides a local conversational implementation of the human-judgment method. The hosted Socrates GitHub App is a separate system of record that can authenticate GitHub accounts, bind activity to commits, manage follow-ups, and issue signed records. A local skill receipt is not an official Socrates stamp.

## Project policies

- [Evaluation](EVALUATION.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)
- [Brand policy](BRAND.md)
- [Apache-2.0 license](LICENSE)
