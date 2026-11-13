# Evidence Handling

Evidence is not decoration; it is the basis for every technical claim.

## Accepted evidence

- Sanitized screenshots
- Redacted request/response logs
- Exact test cases and expected outcomes
- Configuration snapshots without secrets
- Test runner output
- Reproduction instructions

## Naming convention

`YYYY-MM-DD_assessment-id_test-id_evidence-type.ext`

Example: `2026-11-13_A01_T03_output-log.txt`

## Integrity and privacy

- Never commit API keys, tokens, passwords, cookies, or private data.
- Use synthetic test content.
- Redact identifiers that could expose a person or organization.
- Keep confidential raw evidence outside the public repository.
- Record enough context to reproduce the result without exposing secrets.

No evidence has been collected yet.
