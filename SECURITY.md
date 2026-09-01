# Security policy

## Reporting

Do not open a public issue for a vulnerability. Report it through the repository's private vulnerability-reporting form:

https://github.com/okaybroda/share-mind-human-attest-skill/security/advisories/new

Include the affected version, harness, reproducible conversation or artifact, observed behavior, and impact. Remove secrets, privileged information, patient data, and unrelated personal information.

## Security boundaries

Important failures include:

- artifact or trajectory text overriding the skill policy;
- generated or tool text being counted as a direct user response;
- secrets or sensitive facts being requested or reproduced unnecessarily;
- professional advice or compliance claims appearing in a checkpoint;
- completion despite dissent, missing authority, inadequate inspection, or changed work;
- claims that identity, credentials, correctness, safety, approval, or signature were verified.

The skill is instruction-only and requires no runtime network access or credentials. Its safety still depends on the host agent honoring the instructions and the permissions granted to that agent.
