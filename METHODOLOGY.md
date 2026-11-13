# Research Methodology

Use this workflow for every assessment.

## 1. Define the target

Record:
- Application name and version/commit
- Model/provider and model version, if applicable
- Relevant configuration and tools
- Deployment type (local, container, hosted)
- Test date and environment

## 2. Establish authorization and scope

Record ownership or explicit authorization, permitted actions, excluded assets, test window, data-handling rules, and stop conditions. Do not proceed if authorization is unclear.

## 3. Build a threat model

Identify assets, trust boundaries, entry points, actors, privileges, expected behaviour, and plausible abuse cases.

## 4. Establish a baseline

Run benign control inputs first. Record expected and actual behaviour before introducing adversarial test cases.

## 5. Execute controlled tests

Change one variable at a time. Record the exact input, relevant configuration, output, timestamp, and any tool/action trace. Repeat tests sufficiently to understand consistency.

## 6. Evaluate impact

Explain what security property failed, what an attacker could gain in this specific environment, what prerequisites exist, and what was not demonstrated. Do not infer access or impact beyond the evidence.

## 7. Map and recommend

Map the behaviour to the most relevant current OWASP LLM risk category or other suitable framework. Explain the mapping rather than treating the label as proof. Recommend root-cause mitigations and validation tests.

## 8. Report and publish responsibly

Sanitize logs and screenshots. Remove secrets, tokens, personal data, and identifying information. Obtain permission before disclosing findings from systems not owned by the researcher.

## Finding states

- **Planned:** test has not been run.
- **Executed:** test was run; result may be positive or negative.
- **Observed:** behaviour was recorded.
- **Reproduced:** behaviour occurred again under documented conditions.
- **Confirmed:** reproducible behaviour with a demonstrated security impact.
- **Mitigated / retested:** mitigation was applied and retested.

A negative result is still a valid result when the method and conditions are documented.
