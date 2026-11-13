# AI Security Research

**Independent research programme | Learning, experimentation, and reproducible security assessment**

This repository documents practical research into the security of generative AI applications, large language models (LLMs), retrieval-augmented generation (RAG), and agentic systems.

The goal is to develop and demonstrate the ability to understand AI application architectures, design controlled security tests, reproduce observed weaknesses, assess impact, and recommend mitigations.

> **Research integrity:** This repository begins as a learning and experimental programme. It does not claim professional engagements, certifications, successful exploits, or validated vulnerabilities unless supported by evidence in the relevant assessment.

## Research principles

- Test only systems you own, intentionally vulnerable training environments, or systems for which you have explicit written authorization.
- Define scope and rules of engagement before testing.
- Separate hypotheses, observations, and confirmed findings.
- Preserve reproducible test inputs, outputs, configurations, and logs.
- Document unsuccessful tests as well as successful ones.
- Do not publish secrets, personal data, client information, or exploit details that could enable harm.
- Prefer mitigations that address root causes rather than relying only on prompt wording.

## Research divisions

| Division | Focus | Status |
|---|---|---|
| 01. Foundations | HTTP, APIs, Python, application security, threat modelling | Planned |
| 02. LLM security | Prompt injection, jailbreaks, information disclosure, multimodal inputs | Planned |
| 03. Agent security | Tool misuse, excessive agency, permissions, memory and delegation | Planned |
| 04. AI infrastructure | RAG, vector stores, data boundaries, integrations | Planned |
| 05. Red-team methodology | Test design, repeatability, automation, evaluation | Planned |
| 06. Defensive engineering | Least privilege, validation, isolation, monitoring and mitigations | Planned |
| 07. Research publications | Technical reports, case studies and responsible disclosure | Planned |

## Initial assessment roadmap

1. Direct prompt injection
2. Indirect prompt injection
3. Jailbreaking and guardrail bypass
4. System prompt exposure
5. AI agent tool misuse and excessive agency
6. RAG and vector-store data boundary testing
7. Multimodal prompt injection
8. Memory and context isolation testing

These are research topics, not claims that vulnerabilities have been found.

## Repository structure

```text
ai-security-research/
├── README.md
├── RESEARCH_CHARTER.md
├── METHODOLOGY.md
├── .gitignore
├── lab-environment/
│   ├── scope-and-rules.md
│   ├── setup.md
│   └── architecture.md
├── assessments/
│   ├── 01-direct-prompt-injection/
│   ├── 02-indirect-prompt-injection/
│   ├── 03-jailbreaking-guardrail-bypass/
│   ├── 04-system-prompt-exposure/
│   ├── 05-agent-tool-misuse/
│   ├── 06-rag-data-boundaries/
│   ├── 07-multimodal-injection/
│   └── 08-memory-context-isolation/
├── reports/
│   └── REPORT_TEMPLATE.md
├── evidence/
│   └── README.md
├── scripts/
├── references/
│   └── README.md
└── journal/
    └── research-log.md
```

## Assessment status

| Assessment | Status |
|---|---|
| Direct prompt injection | Not started |
| Indirect prompt injection | Not started |
| Jailbreaking / guardrail bypass | Not started |
| System prompt exposure | Not started |
| Agent tool misuse | Not started |
| RAG data boundaries | Not started |
| Multimodal injection | Not started |
| Memory / context isolation | Not started |

## How to read this portfolio

Each assessment should contain:
- `README.md` — objective, scope, threat model and test plan
- `test-cases.md` — exact test cases and expected outcomes
- `results.md` — observed outcomes, including failures
- `evidence/` — sanitized logs and screenshots, where appropriate

A result is **confirmed** only when the observed behaviour is repeatable and its security impact is demonstrated within the authorized test environment.

## Research references

- OWASP GenAI Security Project: https://genai.owasp.org/
- OWASP Top 10 for LLM Applications: https://genai.owasp.org/llm-top-10/
- OWASP AI Testing Guide: https://owasp.org/www-project-ai-testing-guide/
- Promptfoo documentation: https://www.promptfoo.dev/docs/
- MITRE ATLAS: https://atlas.mitre.org/

## Researcher

Independent AI security researcher in training.

This repository is a public record of learning and practical research. Claims about experience and findings will be updated only when supported by verifiable work.
