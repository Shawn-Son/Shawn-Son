# Minhyeok (Shawn) Son

**M.S. Data Science, University of Michigan · new grad, May 2027** · F-1, 36-month STEM OPT, no sponsorship needed at hire

I build ML and LLM systems and measure whether they work: an LLM triage agent in production at eBay, a *Scientific Reports* paper on cheaper fault prediction, and an open-source profiler for coding-agent token spend.

---

## Experience

**eBay** · Machine Learning Engineer Intern · May–Aug 2026 · *internal, no public code*
Built an LLM triage agent for production alerts. Giving it known false-positive cases as exemplars cut false positives from **40% to 10%** of alerts. Pre-triage shortened a **22**-step alert response to **9**, saving **10 hrs/week**.

**University of Michigan × American Airlines** · Student ML Engineer · Sep–Nov 2025
Joined operations, weather and congestion data for **1M+** flights into a PostgreSQL feature store. An XGBoost + random-forest ensemble cut delay-minute RMSE from **11.23 to 3.78**.

**Industrial AI Lab, SeoulTech** · Research Assistant · 2022–2024
Rare-defect detection on manufacturing sensor data, which led to the paper below.

## Research

**[Active Inspection with Knowledge Distillation for Cost-Effective Fault Prediction](https://www.nature.com/articles/s41598-026-39412-8)** · Heo, **Son**, Shim · *Scientific Reports* 16, 8613 (2026) · [code](https://github.com/Shawn-Son/Knowledge-Distillation-for-cost-effective-fault-Prediction-in-manufacturing-process)
On **~263K** semiconductor units with a **<2%** defect rate, a student model trained on cheap features matched a teacher that needs costly inspection data. Uncertainty sampling beat random inspection by **3 AUC points**.

## Competition

**eBay University ML Competition: 3rd of 80, solo** · [leaderboard](https://eval.ai/web/challenges/challenge-page/2508/leaderboard/6263)
Attribute extraction from **10K** German listing titles with XLM-R / mDeBERTa and a word-level CRF. Finished **0.002** behind first place on the official precision-weighted F<sub>β</sub>.

## Open source

**[agentprof](https://github.com/Shawn-Son/agentprof)**: shows where Claude Code tokens and dollars go · *Node.js, zero dependencies* · [![test](https://github.com/Shawn-Son/agentprof/actions/workflows/test.yml/badge.svg)](https://github.com/Shawn-Son/agentprof/actions/workflows/test.yml)
Every context token is assigned to one of **7** waste kinds (stale context, duplicate reads, oversized tool output, unused MCP tools, cache misses, filler, retries), priced with cache-aware rates, and split into confirmed and estimated. A background indexer keeps the status line at about 25 ms per update. **16** black-box tests run the real CLI on synthetic transcripts in CI (Ubuntu and macOS, Node 18/20/22).

```
◆ Opus 5 │ ctx 41% │ 5h 34% · 7d 12% │ ≈ today $2.14 · 7d $18.3 · 30d $71.0
◇ waste $0.81 (38%: confirmed 24% + est 14%) │ stale 22% · tool-out 9% · MCP 7%
```

**[AutoML Service](https://github.com/Shawn-Son/Auto-ML-Service)**: no-code Streamlit app for tabular data · *Python* · [demo](https://youtu.be/rONjcUmTDWk)
Upload a CSV, and it detects the task type (classification, regression or time series), then runs EDA, preprocessing, a grid search over scikit-learn / XGBoost / LightGBM / Prophet candidates, and a downloadable SHAP report.

<sub>Earlier research code: [dysarthric speech classification with calibration](https://github.com/Shawn-Son/Classification_and_Calibration_of_Dysarthric_Speech) (94.4% acc, 1.5% ECE) · [knowledge distillation × calibration on long-tailed CIFAR](https://github.com/Shawn-Son/Optimal-Combination-of-Knowledge-Distillation-and-Calibration-Techniques-for-Reliable-AI-Models) · [time-series fault detection](https://github.com/Shawn-Son/Fault-Point-Labeling-and-Fault-Detection-in-Time-Series-Data)</sub>

---

**Skills**: Python, SQL, Java · PyTorch, scikit-learn, XGBoost, Transformers, LLM agents / RAG, knowledge distillation, calibration · FastAPI, Docker, Streamlit, SHAP

[shawn22587@gmail.com](mailto:shawn22587@gmail.com) · [linkedin.com/in/minhyeokson](https://www.linkedin.com/in/minhyeokson) · [minhyeokson-com.vercel.app](https://minhyeokson-com.vercel.app)
