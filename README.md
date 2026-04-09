# Commerce Ops Agent (Public Showcase)

This is the **public showcase edition** of a production-style e-commerce Agent project.

To protect commercial confidentiality, this repository only includes:

- product overview
- system architecture
- API workflow design
- feature descriptions and demo contracts

It intentionally excludes:

- core business source code
- private scripts and automation logic
- internal data processing rules
- production credentials, mappings, and operational details

## Project Overview

This project is a conversational operations assistant for e-commerce workflows, including:

1. inventory and market query routing
2. conversational operation drafting (listing / repricing in dry-run mode)
3. two-platform profit comparison with downloadable report
4. RAG-based retrieval for SKU resolution under natural language input

## Technical Direction

- Backend framework: FastAPI-style service architecture
- Agent design: tool-based routing with explainable tool calls
- Retrieval: heavy RAG strategy (Embedding + Vector DB + Rerank + fallback)
- Reporting: structured comparison output + downloadable CSV pipeline
- Frontend integration: userscript-based panel integration design

## Repository Structure

- `docs/ARCHITECTURE.md`: architecture and workflow
- `docs/FEATURES.md`: core feature modules
- `docs/API_CONTRACT.md`: public API contract and demo examples
- `docs/SECURITY_AND_SCOPE.md`: confidentiality boundary and publish scope
- `docs/RESUME_DESCRIPTION.md`: ready-to-use resume/project description text
- `PUBLISH_STEPS.md`: publish steps (English)
- `PUBLISH_STEPS_CN.md`: publish steps (Chinese)

## Notes

This repository is for portfolio and communication purposes only.
