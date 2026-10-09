# AI Portfolio Intelligence - AI Handoff Pack

**Status:** Planning / proposed architecture (not implemented)
**Context as of:** 2026-10-09

This folder transfers a product discussion to another AI assistant or coding agent. It is **not** a record of implemented features, successful benchmarks, user validation, or finalized architecture.

## Read order

1. `docs/PROJECT_CONTEXT.md` - why the project exists, requirements, current thinking, constraints.
2. `docs/DECISIONS.md` - confirmed product requirements vs proposed technical choices vs open questions.
3. `docs/PRD.md` - product behavior, user journeys, acceptance criteria, non-goals.
4. `docs/ARCHITECTURE.md` - suggested components, data boundaries, AI integration and operational caveats.
5. `docs/ROADMAP.md` - staged implementation and exit criteria.

## Prompt to paste into a new AI chat

> Read all files in `docs/`, starting with `PROJECT_CONTEXT.md` and `DECISIONS.md`. Continue designing the public AI Portfolio Intelligence Platform. Do not treat tentative technology recommendations as locked decisions. Do not invent product decisions or implementation status. For each suggestion, state what is already agreed, what you propose, trade-offs, and anything that needs validation. Respond in Thai unless asked otherwise.

## Essential guardrails

- Financial amounts, P&L, cash flows, rebalancing and risk metrics must be calculated by deterministic code, not by an LLM.
- Screenshot extraction is provisional until the user verifies it; missing fields must never be hallucinated.
- Snapshot imports and transactions are separate concepts and must not be double-counted.
- Personal holdings, statements, thesis, and embeddings require per-user authorization, not just filtering in the UI.
- AI "memory" means storing and retrieving information, **not** unattended continuous weight training.
- This is a planned public web product. Requirements for market-data redistribution, privacy, and regulated investment advice must be checked before launch.

## Updating the pack

Update `docs/DECISIONS.md` whenever a product/architecture decision changes, and then synchronize the other files. Keep unresolved matters clearly marked as unresolved.
