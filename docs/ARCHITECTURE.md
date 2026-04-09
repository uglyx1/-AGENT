# Architecture

## High-Level Flow

1. User sends natural language request to `/chat`.
2. Intent router decides which tool chain to trigger.
3. If SKU is missing, retrieval module resolves candidate SKUs.
4. Selected tool executes (query / compare / draft operation).
5. Agent returns:
   - answer summary
   - tool call trace
   - structured payload for UI rendering

## Agent Layers

- API Layer
  - health, chat, compare-report, download endpoints
- Orchestration Layer
  - intent parsing
  - tool selection
  - fallback routing
- Tool Layer
  - inventory query tool
  - market query tool
  - profit compare/report tool
  - listing/repricing draft tool (dry-run only)
- Retrieval Layer
  - exact match first
  - embedding retrieval via vector DB
  - rerank on top candidates
  - TF-IDF fallback for resilience

## Reliability Strategy

- deterministic fallback when external retrieval services are unavailable
- dry-run safety mode for high-risk operations
- structured response contract for debuggability and trust

