# Lab Scope and Rules of Engagement

## Authorized targets

Testing is limited to:
1. Applications and infrastructure owned and controlled by the researcher.
2. Intentionally vulnerable training labs whose terms permit the planned tests.
3. Systems covered by explicit written authorization that identifies the assets and permitted testing.

## Prohibited activity

- Testing public or third-party systems without permission
- Accessing, collecting, or disclosing real users' private information
- Attempting persistence, destructive actions, denial of service, or lateral movement
- Sending unauthorized messages or triggering real-world transactions through tools
- Using real credentials, secrets, or production data in test prompts
- Publishing confidential findings without authorization

## Safe test data

Use synthetic names, documents, accounts, API keys, and records. Any credentials used in a local lab must be dummy values with no access to real services.

## Stop conditions

Stop immediately if:
- The test leaves the defined lab boundary
- Real personal or confidential data appears
- An action could affect a real user, account, payment, or external service
- Unexpected access to another tenant or system is observed
- Authorization or scope becomes uncertain

## Evidence handling

Store only sanitized evidence. Keep raw sensitive evidence out of the public repository. Do not commit `.env` files, API keys, tokens, private reports, or customer data.
