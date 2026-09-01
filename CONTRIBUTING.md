# Contributing

Contributions that improve the universal human-judgment policy, portability, safety boundaries, or observable evaluations are welcome.

## Design constraints

- Keep one domain-neutral runtime policy in `SKILL.md`.
- Do not add domain-specific runtime prompts or answer formulas.
- Do not add provider, network, MCP, GitHub, or executable dependencies to the core skill.
- Preserve one-question-at-a-time behavior and one focused follow-up per question.
- Preserve dissent and fail-closed completion.
- Do not expand the completion claim beyond the direct conversational evidence.

## Pull requests

Explain the observed failure that motivates the change and add or update a scenario in `EVALUATION.md`. Evaluate behavior, not exact generated wording. Run the standard skill validator before submitting.

Changes that weaken privacy, professional-advice boundaries, prompt-injection resistance, or completion limitations require explicit security review.
