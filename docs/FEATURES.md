# Feature Modules

## 1. Conversational Query Agent

- accepts natural language requests
- supports inventory and market lookup scenarios
- can resolve incomplete product references using retrieval

## 2. Heavy RAG Retrieval

- embedding-based semantic retrieval for noisy/unstructured input
- vector database candidate recall
- rerank stage for precision optimization
- TF-IDF fallback for low-dependency continuity

## 3. Two-Platform Profit Comparison

- compares current-platform price baseline against second-platform feed
- filters by profit threshold (example: profit > 100 / 200)
- returns both preview table and downloadable report metadata

## 4. Report Export and Download

- structured result rows
- CSV export pipeline
- direct download endpoint contract for UI consumption

## 5. Operation Draft Mode (Safety First)

- conversational listing/repricing planning
- parameter completeness checks
- explicit dry-run response (`executed=false`)
- no real write operation in public demo scope

