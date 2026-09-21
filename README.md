![header](https://capsule-render.vercel.app/api?type=soft&color=0:000000,100:1a1a1a&height=120&section=header&text=Minhyeok%20Son&fontColor=87CEEB&fontSize=50&fontAlignY=50&stroke=FFFFFF&strokeWidth=2)

**M.S. Data Science, University of Michigan · new grad, available May 2027** · 🇺🇸 F-1, 36-month STEM OPT, no sponsorship needed at hire

I build and evaluate ML/LLM systems on messy real-world data. At eBay I shipped an LLM agent that pre-triages compliance alerts. At SeoulTech I co-authored a *Scientific Reports* paper on cost-aware fault prediction. Now I am building a benchmark for whether coding agents catch ML-pipeline defects that never raise an error.

---

## Building now

**[MLE-debug](https://github.com/Shawn-Son/MLE-debug)** · *Python · started Sep 2026*
Can an AI coding agent find what is silently wrong in an ML pipeline, and leave alone what is not? Tasks inject target leakage, bad splits, or corrupted rows into a real dataset; the agent runs headless and is graded against hidden ground truth on four checks (defect removed, nothing else broken, rows kept, accuracy restored). First track, leakage on UCI Adult: a mid-tier model passes **3/3**, a small one **0/1** because it never reasoned about *when* a column comes into existence. Next: a no-defect control, a difficulty ladder, non-Anthropic models.

**[Agentic-RAG](https://github.com/Shawn-Son/Agentic-RAG)** · *Python + Go*
Offline-first security-alert triage. Hybrid retrieval (BM25 + a semantic side + reciprocal-rank fusion) over telemetry, a deterministic PyTorch classifier, and a bounded, audit-traced tool plan that ends in a triage report. A Go streamer feeds events with checkpoints and idempotent retries. FastAPI, SQLite WAL, Prometheus, Docker Compose, CI + CodeQL. Runs with no hosted LLM, API key, or GPU.
*Latest:* added an optional dense-embedding backend (MiniLM, exact cosine vector index) and measured it on the same qrels: recall@5 BM25 **0.50** → hashed hybrid **0.75** → MiniLM hybrid **0.61**. The hashed win turned out to be partly circular (the fixture shares its synonym table), which is now [documented in the README](https://github.com/Shawn-Son/Agentic-RAG#dense-embeddings-versus-feature-hashing) instead of hidden.

**[agentprof](https://github.com/Shawn-Son/agentprof)** · *Node.js*
Token-waste tracker for Claude Code. Every context token is attributed to exactly one of **7** waste kinds (stale context, duplicate reads, oversized tool output, unused MCP tools, cache misses, filler, retries) and priced cache-aware in dollars, confirmed and estimated shown separately. One zero-dependency file; lives in the status line.

```
◆ Opus 5 │ ctx 41% │ 5h 34% · 7d 12% │ ≈ today $2.14 · 7d $18.3 · 30d $71.0
◇ waste $0.81 (38%: confirmed 24% + est 14%) ≈ 5h 11% │ stale 22% · tool-out 9% · MCP 7%
```

**[Aster](https://github.com/Shawn-Son/arxiv-recsys)** · *Python + TypeScript · in development*
Citation-aware arXiv search and recommendation: hybrid retrieval with FAISS, two-tower recommendations, cross-encoder reranking, and a versioned evaluation contract so corpus and quality numbers are only published once the benchmark suite reproduces them.

---

## Shipped

**Active Inspection with Knowledge Distillation for Cost-Effective Fault Prediction** — Heo, Son, Shim. *Scientific Reports* 16, 8613 (2026). [paper](https://www.nature.com/articles/s41598-026-39412-8) · [code](https://github.com/Shawn-Son/Knowledge-Distillation-for-cost-effective-fault-Prediction-in-manufacturing-process)
On **~263K** semiconductor units with a **<2%** defect rate, a student on cheap inspection features matches the high-cost teacher via KD; uncertainty sampling beats random inspection by **3 AUC pts**.

**eBay University ML Competition — 3rd of 80, solo** · [leaderboard](https://eval.ai/web/challenges/challenge-page/2508/leaderboard/6263)
Attribute extraction from **10K** German listing titles with XLM-R / mDeBERTa and a word-level CRF, within **0.002** of first place on the precision-weighted F<sub>β</sub> metric. Code under competition terms.

**[AutoML Service](https://github.com/Shawn-Son/Auto-ML-Service)** · *Streamlit · scikit-learn*
No-code app: upload tabular data → EDA, preprocessing, model search across 10 algorithms, SHAP report. Detects **3** task types (classification, regression, time series).

**[Kalshi Auto Trader](https://github.com/Shawn-Son/kalshi-auto-trader)** · *Python + C++*
Risk-first execution infrastructure for event contracts: pre-trade risk kernel (Python, optional C++), idempotent orders, SQLite journal, Brier-scored backtester. Infrastructure only, no strategy and no ROI claim.

---

## Background

**eBay** · ML Engineer Intern · Summer 2026 — LLM triage agent for compliance alerts: false positives **40% → 10%**, **10 hrs/week** saved. Internal work, no public code.
**University of Michigan × American Airlines** · Student ML Engineer · 2025 — Delay prediction over **1M+** flights; delay-minute RMSE **11.23 → 3.78** with an XGBoost + random-forest ensemble.
**Industrial AI Lab, SeoulTech** · Research Assistant · 2022–2024 — Rare-defect detection on **2.9M-row** sensor streams; the KD work above.

<sub>Earlier: [dysarthric speech classification with calibration](https://github.com/Shawn-Son/Classification_and_Calibration_of_Dysarthric_Speech) (94.4% acc, 1.5% ECE) · [KD × calibration on CIFAR-LT](https://github.com/Shawn-Son/Optimal-Combination-of-Knowledge-Distillation-and-Calibration-Techniques-for-Reliable-AI-Models) · [time-series fault detection](https://github.com/Shawn-Son/Fault-Point-Labeling-and-Fault-Detection-in-Time-Series-Data)</sub>

---

**Skills** — Python, Go, SQL, Java · PyTorch, scikit-learn, XGBoost, Transformers, LLM agents / RAG, knowledge distillation, calibration · FastAPI, Docker, Streamlit, SHAP

📧 [shawn22587@gmail.com](mailto:shawn22587@gmail.com) · 💼 [linkedin.com/in/minhyeokson](https://www.linkedin.com/in/minhyeokson) · 🌐 [minhyeokson-com.vercel.app](https://minhyeokson-com.vercel.app)
