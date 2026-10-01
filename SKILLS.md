# Prebid.js — Skills & Capabilities

## Role
**Frontend Sub-Agent (Role C)** — Prebid.js fork with custom adpulse modules.

## Primary Capabilities
- Prebid.js fork with custom bidder adapters and analytics modules
- Global variable namespace: `adppbjs` (not standard `pbjs`)
- Gulp build pipeline with ESLint code quality checks
- Integration with adp-publisher-tag for GPT + Prebid auction strategies

## LightRAG Collection
LightRAG has ONE workspace, `adpulse` (no per-repo collections). Query via `mcp__lightrag-mcp__query` / `query_context` with the repo name (`Prebid.js`) in the query; see [../AGENTS.md](../AGENTS.md) (hub) and this repo's AGENTS.md "LightRAG-first workflow" section.

## Agent Skills to Activate
*(none — Prebid.js development, no special skills required)*

## Key Constraints
- **Branch naming** *(upstream-only rule, from the upstream Prebid.js AGENTS.md; not applicable to the AdPulse fork)*: branch names include 'codex' or 'agent'
- **Global var**: always use `adppbjs` (not `pbjs`)
- **PR messages**: follow Prebid.js community guidelines *(upstream-only: the bot-comment / fruit-named-function rules apply to PRs against `prebid/Prebid.js`, not the AdPulse fork)*
- **Test before PR**: run `gulp test --file` for changed modules
- This is a **fork** of upstream Prebid.js — merge conflicts with upstream must be handled carefully

## References
- [AGENTS.md](./AGENTS.md) — Full architecture, build commands, PR guidelines, agent detection clause
