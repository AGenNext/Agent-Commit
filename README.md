# Agent-Commit

Agent-Commit owns commit, branch, pull request, and merge preparation for AGenNext repositories.

## Governance Boundary

Agent-Commit does not define governance rules.

Agent-deploy owns validation, CI/CD, deployment, and post-deployment production sanity. Agent-Commit must consume Agent-deploy validation before commit, pull request, merge, promotion, or release preparation.

## Required Validation Flow

Before Agent-Commit sends any change toward AGenNext servers:

1. Run edge/client-side validation in the user's browser/client where available.
2. Run Agent-deploy governance validation against the target repository.
3. Attach validation evidence to the commit or pull request.

## Language Boundary

Outside SurrealDB, SurrealQL, SurrealML, and AgentQL, the only approved implementation language is browser-side TypeScript.

TypeScript is the single FE/UI language so browser authoring, validation, and execution stay in one toolchain without code conversion. This keeps the UI surface aligned with current frontend development practice and supports fast edge delivery.

## Central Source

Editable validation rules live in Agent-deploy:

```text
AGenNext/Agent-deploy/governance/
```
