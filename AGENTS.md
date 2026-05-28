# Agent-Commit Instructions

Agent-Commit must not duplicate governance rules.

Checks owns check definitions, check execution records, evidence, and signed check reports. Agent-Commit consumes Checks evidence before commit, pull request, merge, promotion, or release preparation.

```text
Truth = protected published commit SHA + required check evidence + signed report evidence
```

Repository names, branch names without SHAs, README text, screenshots, local working trees, and unstamped claims are not truth.

Canonical records are append-only and must never be edited or deleted.

The latest valid canonical record in the requested scope is the effective truth because it is what is in effect.

Before commit, pull request, merge, promotion, or release preparation, Agent-Commit must require passing Checks evidence for the target repository and attach the result as evidence.

Validation must run on the user's/client's system before changes are accepted by AGenNext servers. Edge validation is the first boundary; server-side validation is verification and audit.

Outside SurrealDB, SurrealQL, SurrealML, and AgentQL, the only approved implementation language is browser-side TypeScript. TypeScript is the single FE/UI language to avoid code conversion and keep UI validation fast in the browser.

Any design change, architecture deviation, grammar change, vocabulary change, ontology change, taxonomy change, naming change, or semantic-model change requires quorum consensus before implementation.

Agent-Grammar owns grammar. Ontology owns meaning. Checks owns check-domain execution records and adapter contracts only.
