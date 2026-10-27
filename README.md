# Minhyeok (Shawn) Son

**M.S. Data Science, University of Michigan · new grad, May 2027** · 🇺🇸 F-1, 36-month STEM OPT, no sponsorship needed at hire

I build and evaluate ML/LLM systems on messy real-world data: an LLM triage agent shipped at eBay, a *Scientific Reports* paper on cost-aware fault prediction, and a profiler that shows where a coding agent's tokens went.

---

## Projects

**[agentprof](https://github.com/Shawn-Son/agentprof) — Token-waste tracker for Claude Code, in dollars, in your status line.** · *Node.js*
Every context token attributed to one of **7** waste kinds (stale context, duplicate reads, oversized output, unused MCP tools, cache misses, filler, retries); confirmed vs estimated shown separately. One zero-dependency file, installs as a skill.

```
◆ Opus 5 │ ctx 41% │ 5h 34% · 7d 12% │ ≈ today $2.14 · 7d $18.3 · 30d $71.0
◇ waste $0.81 (38%: confirmed 24% + est 14%) │ stale 22% · tool-out 9% · MCP 7%
```

---

## Shipped

**[Active Inspection with Knowledge Distillation](https://www.nature.com/articles/s41598-026-39412-8)** — Heo, Son, Shim. *Scientific Reports* 16, 8613 (2026) · [code](https://github.com/Shawn-Son/Knowledge-Distillation-for-cost-effective-fault-Prediction-in-manufacturing-process)
**~263K** semiconductor units, **<2%** defect rate: KD student on cheap features matches the high-cost teacher; uncertainty sampling beats random by **3 AUC pts**.

**eBay University ML Competition — 3rd of 80, solo** · [leaderboard](https://eval.ai/web/challenges/challenge-page/2508/leaderboard/6263)
Attribute extraction from **10K** German listing titles (XLM-R / mDeBERTa + word-level CRF), **0.002** behind first on precision-weighted F<sub>β</sub>.

**[AutoML Service](https://github.com/Shawn-Son/Auto-ML-Service)** — no-code Streamlit app: upload tabular data → EDA, preprocessing, search over 10 algorithms, SHAP report; **3** task types.

---

## Background

**eBay** · ML Engineer Intern · Summer 2026 — LLM triage agent: false positives **40% → 10%**, **10 hrs/week** saved. Internal, no public code.
**UMich × American Airlines** · Student ML Engineer · 2025 — delay prediction over **1M+** flights, RMSE **11.23 → 3.78**.
**Industrial AI Lab, SeoulTech** · Research Assistant · 2022–2024 — rare-defect detection on **2.9M-row** sensor streams → the paper above.

<sub>Earlier: [dysarthric speech calibration](https://github.com/Shawn-Son/Classification_and_Calibration_of_Dysarthric_Speech) (94.4% acc, 1.5% ECE) · [KD × calibration on CIFAR-LT](https://github.com/Shawn-Son/Optimal-Combination-of-Knowledge-Distillation-and-Calibration-Techniques-for-Reliable-AI-Models) · [time-series fault detection](https://github.com/Shawn-Son/Fault-Point-Labeling-and-Fault-Detection-in-Time-Series-Data)</sub>

---

**Skills** — Python, SQL, Java · PyTorch, scikit-learn, XGBoost, Transformers, LLM agents / RAG, knowledge distillation, calibration · FastAPI, Docker, Streamlit, SHAP

📧 [shawn22587@gmail.com](mailto:shawn22587@gmail.com) · 💼 [linkedin.com/in/minhyeokson](https://www.linkedin.com/in/minhyeokson) · 🌐 [minhyeokson-com.vercel.app](https://minhyeokson-com.vercel.app)
