## Hi, I'm MD Minhazur Rahman 👋

**Data Scientist / ML Engineer** — I build production-grade ML systems end to end: cloud-deployed services, streaming pipelines, orchestrated retraining, experimentation tooling, and LLM agents.

🎓 MSc Data Science, University of Greenwich · 3+ years across data & IT roles
🌍 Based in Bangladesh · open to **Data Scientist / ML Engineer roles worldwide**, including visa sponsorship & relocation (EU Blue Card eligible · GCC · UK)

🌐 **Portfolio: [minhazda.github.io](https://minhazda.github.io)** · 📄 [CV (PDF)](https://github.com/minhazda/cv/raw/main/CV_MD_MinhazurRahman.pdf)

---

### ▶ Live demos — deployed on GCP Cloud Run

*Both scale to zero: the first request after idle takes ~10s to wake.*

**[fraud-detection-mlops](https://github.com/minhazda/fraud-detection-mlops)** — *Imbalanced classification, deployed*
Real-time card-fraud scoring: LightGBM with class-imbalance handling, a validation-tuned decision threshold, and raw-transaction feature engineering shared between training and serving (no train/serve skew).
📈 **ROC-AUC 0.90 · PR-AUC 0.49 (~8× the base rate)** · ▶ **[Try the live demo](https://fraud-detection-api-ude5vos6lq-uc.a.run.app/)** — enter a transaction, get a risk score

**[synthetic-retail-mlops-pipeline](https://github.com/minhazda/synthetic-retail-mlops-pipeline)** — *Production MLOps, deployed*
Retail demand forecasting re-engineered into a deployable service: Docker, MLflow, FastAPI, full CI/CD, Terraform IaC, Prometheus/Grafana + Evidently drift monitoring. Typed, tested, reproducible.
📈 **LightGBM cut MAE 40.8% / RMSE 47.3%** vs the naïve baseline · ▶ **[Try the live demo](https://retail-forecasting-api-ude5vos6lq-uc.a.run.app/)** — set conditions, get a forecast

### 🔁 Streaming, orchestration & experimentation

**[streaming-fraud-detection](https://github.com/minhazda/streaming-fraud-detection)** — *Event-driven ML*
Kafka/Redpanda stream processor scoring transactions in real time with the fraud model: strict schema validation into a dead-letter queue, alerts topic, Prometheus scoring-latency histograms. Written against a `MessageBus` protocol so the full pipeline unit-tests without a broker — then **CI runs the same pipeline end-to-end against a real Redpanda broker and deploys it onto a kind Kubernetes cluster on every push**.

**[retail-demand-platform](https://github.com/minhazda/retail-demand-platform)** — *Orchestrated data + ML pipelines*
Dagster assets → dbt star schema on DuckDB (data tests run as a pipeline stage) → weekly LightGBM retrain on **1M+ real retail transactions**, gated by a champion/challenger promotion rule: a new model ships only on a ≥1% holdout-MAE improvement, with champion metrics versioned in git.

**[experiment-analysis-toolkit](https://github.com/minhazda/experiment-analysis-toolkit)** — *Experimentation statistics*
Power analysis, CUPED variance reduction, always-valid sequential testing (mSPRT), Welch/z analysis with CIs — with **property-based tests of the statistical guarantees themselves**: family-wise false-positive rate under continuous peeking, CI coverage over simulation, CUPED variance-safety.

### 📊 Data rigor & LLMs

**[real-retail-forecasting](https://github.com/minhazda/real-retail-forecasting)** — *Real-world data rigor*
Daily demand forecasting on **1.07M real UCI Online Retail II transactions** — every cleaning decision documented as a first-class artifact, a runnable DuckDB SQL analysis, and an honestly-reported PyTorch benchmark (the MLP's small accuracy edge didn't justify 9× the fit time, so LightGBM stays the default).
📈 **+26.3% pooled MAE over seasonal-naïve, beating the baseline on 47/49 series (96%)** · honest metrics, no fabricated numbers.

**[privacy-preserving-rag-agent](https://github.com/minhazda/privacy-preserving-rag-agent)** — *LLM / RAG*
A LangGraph tool-calling agent over a document corpus with on-device embeddings, behind a fail-closed privacy guard (PII redaction + synthetic-only validation).
📈 **Two-tier eval: deterministic CI gate + Claude LLM-as-judge (RAGAS-style) with Langfuse tracing.**

<sub>📄 Research foundation: [synthetic-retail-forecasting](https://github.com/minhazda/synthetic-retail-forecasting) — controllable synthetic-data generator + Rolling-Origin CV of tree ensembles. DOI-indexed: [10.5281/zenodo.19479285](https://doi.org/10.5281/zenodo.19479285)</sub>

### 🤖 Automation & agentic tooling

**[job-radar](https://github.com/minhazda/job-radar)** — *Live demo* — paste any careers page, get every open role scored for fit with a plain-English "why." Built on [Firecrawl](https://github.com/mendableai/firecrawl) (credited). ▶ **[Try it](https://huggingface.co/spaces/Minhazda/job-radar)**

**[invoice-automation](https://github.com/minhazda/invoice-automation)** — OCR → Pydantic + arithmetic validation → DuckDB ledger, with a human-in-the-loop exception queue for anything malformed. 📈 **73.3% straight-through rate** — every malformed invoice caught, none booked.

**[ai-triage-agent](https://github.com/minhazda/ai-triage-agent)** — Classifies support tickets and drafts grounded replies that never invent policy — no match means a safe holding reply flagged for a human, not a guess.

**[rpa-reconciliation-bot](https://github.com/minhazda/rpa-reconciliation-bot)** — Playwright RPA (retry/backoff, screenshot-on-failure) reconciling transactions against a ledger, proven with a real headless-browser end-to-end test.

**[n8n-automation-hub](https://github.com/minhazda/n8n-automation-hub)** — Three versioned, idempotent n8n workflows (lead intake, error-handling + DLQ, weekly reporting) with a Node.js structural validator running in CI.

<sub>Also: [job-hunter-bd](https://github.com/minhazda/job-hunter-bd) — a free public job-search tool for Bangladeshi job seekers (scraper + match scoring + AI CV tailoring).</sub>

---

### ☁️ Cloud-native MLOps
Both demos deploy to **GCP Cloud Run via Terraform** with **keyless CI/CD (Workload Identity Federation)**, **Prometheus/Grafana** metrics, and **Evidently** drift monitoring. The streaming stack additionally ships **Kubernetes manifests proven by a kind smoke test in CI**.

### 🛠️ Tech
Python · LightGBM / XGBoost / scikit-learn · PyTorch · FastAPI · Kafka (Redpanda) · PySpark · Dagster · dbt · DuckDB · SQL · Docker · Kubernetes · Terraform · GCP Cloud Run · MLflow · Prometheus / Grafana · Evidently · LangGraph · ChromaDB · Playwright · n8n · Streamlit · GitHub Actions · pandas / NumPy · pytest / Hypothesis / mypy

### 📫 Reach me
[LinkedIn](https://www.linkedin.com/in/mohammadminhaz/) · 📧 minhazurrahman.ds@gmail.com
