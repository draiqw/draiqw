# Roman Akramov

**AI / ML Engineer · Full-Stack Developer · R&D Researcher**

I work across the whole path a model takes to production: research and post-training on one end,
FastAPI/React services with CI/CD on the other, and rigorous evaluation tying the two together.
Focus areas: LLM pipelines, RAG, OCR-driven document automation, RL post-training.

Author of an open-source LLM evaluation library and a published paper.

---

## What I do

**R&D research** — reinforcement learning and post-training of LLMs (GRPO-style methods, SFT, dLM),
retriever and reranker design, ablation-driven evaluation. First author of the TMBBO preprint, with
two more papers in preparation on self-play RL and RAG.

**AI engineering** — turning research into systems that run: distributed training on multi-GPU
clusters, inference with vLLM, hybrid retrieval, agent tool-calling and MCP, reproducible pipelines
tracked in W&B, MLflow and TensorBoard.

**Full-stack development** — FastAPI backends, React frontends, WebSocket streaming of LLM
responses, Docker and CI/CD, multi-platform delivery from web to Telegram bots to desktop clients.

---

## Selected work

### MSU, Machine Learning Laboratory — R&D Engineer · 2025 — present

**Evaluation-benchkit** — lead developer of an open-source LLM evaluation library: 22 benchmarks
across 7 categories (GSM8K, MATH-500, ToolQA, HarmBench and others) behind a unified backend layer
for vLLM and HF. Added a UI and leaderboard for tracking runs and comparing prompt, model and
pipeline configurations, which cut the cycle time for testing a hypothesis.

**RAG research** — investigated retrievers on top of a RAPTOR tree and fine-tuned LLaDA-8B (SFT)
as a logit-based reranker. Across 37 ablations against a cosine baseline: QuALITY 68.7 → 72.6 acc,
NarrativeQA 6.0 → 24.9 F1, QASPER 11.0 → 28.7 F1.

**SPICE** — designed a self-play training framework for LLMs on PyTorch and vLLM (RLVR, DrGRPO).
Distributed training on 8×A100 (SLURM, FSDP FULL_SHARD, NCCL/NVLink), LoRA hot-swap between
training and rollout instances, per-rank checkpoint and resume for a dual-optimizer setup. Built an
OCR pipeline that extracts content from PDF textbooks and generates pretrain / SFT / RL data with
iterative dataset accumulation in the self-play loop — up to +3 p.p. on GSM8K and MATH-500.

### Waive — Full-Stack Developer (ML + Web) · 2024 — 2026

**Nexus** — SaaS personal knowledge base with RAG. Built the full ingestion pipeline
(PDF/DOCX/PPTX/XLSX parsing, OCR for scans and images, Whisper transcription, web extraction) and
hybrid retrieval combining Elasticsearch BM25 with vector embeddings, plus LLM synthesis with
citations. Shipped to web, Telegram and a Tauri desktop client.

**AUDS / BimChat** — LLM-driven document validation. A pipeline that reads engineering project
files (IFC), matches them against a graph of GOST regulations in Neo4j, validates entities and
attributes through LLM tool-calling / MCP, and auto-generates compliance reports. Designed the
FastAPI backend, React frontend, CI/CD and WebSocket streaming of LLM responses.

**NDS** — improved report-generation throughput 2.5× via pagination, implemented RAG document
search on Elasticsearch, ran code reviews and decomposed tasks for two developers.

**Aurora** — trained a diffusion model for floor-plan generation and built an interior design
module that applies edits from text prompts via an LLM.

---

## Education

**Lomonosov Moscow State University** — Faculty of CMC, Department of MMP · BSc 2023 — 2027
GPA 4.5/5.0, major-track courses 5.0/5.0.

Deep learning, NLP, CV, optimization and classical ML. Implemented a fully connected network in
NumPy from scratch, U-Net / LinkNet for segmentation, a CNN for image classification, RNN / LSTM
for classification and LM generation, Transformers for NER with HPO via Optuna. On the optimization
side: Lasso, subgradient method, ISTA / FISTA, proximal operators in JAX, the EM algorithm for word
alignment, spectral clustering, OpenCV.

---

## Stack

**Languages** — Python, C++, C, SQL, TS/JS. English B2.

**LLMs and RAG** — prompt engineering, hybrid RAG (BM25 + dense), retrievers and rerankers,
OCR-based ingestion, evaluation and A/B testing, agent tool-calling / MCP.
Commercial providers (Anthropic, OpenAI) and open-source models (Llama, Mistral, LLaDA, Qwen).

**ML/DL** — PyTorch, Transformers, HF, vLLM, FSDP, TRL, PEFT/LoRA, scikit-learn.

**Infra and search** — SLURM, Docker, Linux, Nginx, CI/CD; PostgreSQL, Elasticsearch, Neo4j, Redis,
S3, Celery; MLflow, W&B, TensorBoard.

**Web** — FastAPI, React, WebSocket streaming.

---

## Contact

📍 Moscow · ✉️ [akramovromanr@gmail.com](mailto:akramovromanr@gmail.com) ·
✈️ [t.me/draiqws](https://t.me/draiqws)
