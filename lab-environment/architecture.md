# Planned Lab Architecture

## Components

1. **User interface / request handler:** accepts synthetic user input.
2. **Instruction layer:** holds a simulated system instruction and application policy.
3. **Context loader:** optionally loads synthetic documents.
4. **Assistant logic:** produces a response using deterministic mock behaviour initially.
5. **Tool simulator:** exposes harmless mock tools; it must not call external services or modify real systems.
6. **Audit logger:** records test ID, input, output, and simulated tool decisions without secrets.

## Trust boundaries to examine

- User input versus trusted application instructions
- Retrieved document content versus trusted instructions
- Model-generated tool requests versus application authorization
- One user's synthetic data versus another user's synthetic data
- Conversation history and memory versus current-session state

## Safety properties

- No network egress by default
- No real credentials or customer data
- Tool actions are simulated and allowlisted
- Destructive operations are absent
- Test data is synthetic
- Logs are sanitized before publication

This is a proposed design. It should be updated to match the implementation once the lab is built.
