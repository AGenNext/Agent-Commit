# Agent-Commit Instructions

Agent-Commit must not duplicate governance rules.

Rules are owned by Agent-deploy and consumed from:

```text
AGenNext/Agent-deploy/governance/
```

Before commit, pull request, merge, promotion, or release preparation, Agent-Commit must run Agent-deploy validation against the target repository and attach the result as evidence.

Validation must run on the user's/client's system before changes are accepted by AGenNext servers. Edge validation is the first boundary; server-side validation is verification and audit.

Outside SurrealDB, SurrealQL, SurrealML, and AgentQL, the only approved implementation language is browser-side TypeScript. TypeScript is the single FE/UI language to avoid code conversion and keep UI validation fast in the browser.

Any design change, architecture deviation, grammar change, vocabulary change, ontology change, taxonomy change, naming change, or semantic-model change requires quorum consensus before implementation.
