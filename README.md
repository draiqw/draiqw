# Roman Akramov

**AI/ML Engineer · Full-Stack Developer · R&D @ MSU Machine Learning Lab**

I build LLM systems end to end — post-training and evaluation research on one side, production
FastAPI/React services on the other.

## Research

MSU, Machine Learning Laboratory — R&D Engineer, 2025 — present.

**CRISP / SPICE** — corpus-grounded challenger–reasoner self-play for domain-specific post-training.
Full pipeline: OCR over 766 PDFs → 6.4k-chunk corpus → dual-LoRA self-play → multi-judge curation →
downstream GRPO → 21 benchmarks (EN + RU). 8×A100, SLURM, FSDP, vLLM. Paper plus three released
Russian STEM datasets.

**evaluation-benchkit** — lead developer of the lab's open-source LLM evaluation library: 22
benchmarks across 7 categories (GSM8K, MATH-500, ToolQA, HarmBench), a unified backend layer for
vLLM and HF, and a leaderboard UI for comparing prompt, model and pipeline configurations.

**RAPTOR retrieval** — LLaDA-8B fine-tuned (SFT) as a logit-based reranker over a RAPTOR tree.
Across 37 ablations against a cosine baseline: QuALITY 68.7 → 72.6 acc, NarrativeQA 6.0 → 24.9 F1,
QASPER 11.0 → 28.7 F1.

**Multilingual deep research** — cross-lingual evaluation for deep-research agents: an XBCP scheme
on top of BrowseComp-Plus that translates the document corpus while keeping questions and answers in
English, so answer quality and retriever quality can be measured per language region.

**SAPO** — gate functions for SAPO: custom trainer, cluster training runs and benchmark evaluation
of the resulting checkpoints.

**TMBBO** — first author, preprint. Two more papers in preparation on self-play RL and RAG.

## Production

**DCFP** — automation of a food-production plant, backend and frontend. Batches and batch units,
tech cards with versions and norms, incoming control, inventory and stock, orders and invoices,
disposals, tasting lists, workshops, closing checklists, plans and tasks — plus Excel reporting,
an analytics module and lab quality control. FastAPI, PostgreSQL, Alembic, React, Cypress e2e,
CI/CD and nightly database backups.

**Waive** — startup, ML + full-stack. Selected products:

- **AIVA** — RAG and agent platform: FastAPI, React, Qdrant, Elasticsearch; agent runtime behind an
  MCP server with 12 tools, container-per-run isolation, Bitrix integration, code runner, WebSocket
  streaming of LLM responses.
- **Aiva-router** — LLM routing layer: model registry in the database with pricing and encrypted
  provider keys, per-model enable gate, per-run cost accounting.
- **AUDS / BimChat** — LLM-driven validation of engineering documentation: IFC project files matched
  against a graph of GOST regulations in Neo4j, entities and attributes checked through LLM
  tool-calling / MCP, compliance reports generated automatically.
- **Chebotarev** — interior design service: render generation and editing over Stable Diffusion,
  FLUX, GPT and Gemini, with prompt templates, an LLM quality assessor and upscaling; React Flow
  frontend, FastAPI backend, MinIO storage.
- **Nexus** — SaaS knowledge base with RAG: ingestion (PDF/DOCX/PPTX/XLSX, OCR, Whisper, web
  extraction), hybrid retrieval (BM25 + dense), synthesis with citations; web, Telegram and a Tauri
  desktop client.
- **Nielsen** — document search and deep-research assistant on Yandex AI Studio: FastAPI + Celery
  monorepo, agent runs with skills executed in disposable sandboxes.

## Personal projects

- **drevugol** — production and order management for a charcoal factory (family business): FastAPI,
  PostgreSQL, MinIO, aiogram bot, React, GHCR-based CI/CD.
- **courseplex** — LMS platform (courses, lessons, lesson-linked tests, reviews): React 19, FastAPI,
  ARQ, MinIO; running in production.
- **career-ops** — AI job-search system built on Claude Code: 14 skill modes, Go dashboard, PDF
  generation, batch processing.
- Smaller products, all shipped and deployed: **elagin** (lead management), **slt_service**,
  **calma**, **brainstorm**, **akramfit**, **aero-hockey**.

## Stack

- Python, C++, TS · PyTorch, Transformers, vLLM, FSDP, TRL, PEFT/LoRA
- FastAPI, React, WebSocket streaming · PostgreSQL, Elasticsearch, Neo4j, Qdrant, Redis, MinIO
- SLURM, Docker, CI/CD · MLflow, W&B

## Contact

MSU, Faculty of CMC, Dept. of MMP — BSc 2023–2027 · Moscow ·
[akramovromanr@gmail.com](mailto:akramovromanr@gmail.com) · [t.me/draiqws](https://t.me/draiqws)
