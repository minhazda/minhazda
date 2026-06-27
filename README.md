## Hi, I'm MD Minhazur Rahman 👋

**Data Scientist / ML Engineer** — I turn forecasting, classification & LLM research into production-grade, cloud-deployed ML systems (Docker · Terraform · FastAPI · CI/CD).

🎓 MSc Data Science, University of Greenwich · 3+ years across data & IT roles
🌍 Based in Bangladesh · open to **Data Scientist / ML Engineer roles worldwide**, including visa sponsorship & relocation (EU Blue Card eligible · GCC · UK)

---

### 🚀 Featured projects

**[synthetic-retail-mlops-pipeline](https://github.com/minhazda/synthetic-retail-mlops-pipeline)** — *Production MLOps*
Retail demand forecasting re-engineered into a deployable service: Docker, MLflow tracking, FastAPI serving, full CI/CD, Terraform IaC, Prometheus/Grafana + Evidently observability. Typed, tested, reproducible.
📈 **LightGBM cut MAE 40.8% / RMSE 47.3%** vs the naïve baseline · ▶ **[Live on GCP Cloud Run](https://retail-forecasting-api-ude5vos6lq-uc.a.run.app/health)** (Terraform-deployed)

**[fraud-detection-mlops](https://github.com/minhazda/fraud-detection-mlops)** — *Imbalanced classification (different domain)*
Real-time card-fraud scoring: LightGBM with class-imbalance handling, a validation-tuned decision threshold, and raw-transaction feature engineering at serve time (no train/serve skew).
📈 **ROC-AUC 0.90 · PR-AUC 0.49 (~8× the base rate)** · ▶ **[Live on GCP Cloud Run](https://fraud-detection-api-ude5vos6lq-uc.a.run.app/health)**

**[real-retail-forecasting](https://github.com/minhazda/real-retail-forecasting)** — *Real-world data rigor*
Daily demand forecasting on **1.07M real UCI Online Retail II transactions** — every cleaning decision documented as a first-class artifact, plus a runnable DuckDB SQL analysis reproducing the findings.
📈 **+26.3% pooled MAE over seasonal-naïve, beating the baseline on 47/49 series (96%)** · honest metrics, no fabricated numbers.

**[privacy-preserving-rag-agent](https://github.com/minhazda/privacy-preserving-rag-agent)** — *LLM / RAG*
A LangGraph tool-calling agent over a document corpus with on-device embeddings, behind a fail-closed privacy guard (PII redaction + synthetic-only validation).
📈 **Two-tier eval: deterministic CI gate + Claude LLM-as-judge (RAGAS-style) with Langfuse tracing** · 10-case gold set.

<sub>📄 Research foundation: [synthetic-retail-forecasting](https://github.com/minhazda/synthetic-retail-forecasting) — controllable synthetic-data generator + Rolling-Origin CV of tree ensembles. DOI-indexed: [10.5281/zenodo.19479285](https://doi.org/10.5281/zenodo.19479285)</sub>

---

### ☁️ Cloud-native MLOps
Services deploy to **GCP Cloud Run via Terraform** with **keyless CI/CD (Workload Identity Federation)**, **Prometheus/Grafana** metrics, and **Evidently** drift monitoring.

### 🛠️ Tech
Python · scikit-learn · LightGBM / XGBoost · FastAPI · LangGraph · ChromaDB · Docker · Terraform · GCP Cloud Run · MLflow · Prometheus/Grafana · GitHub Actions · SQL · pandas / NumPy

### 📫 Reach me
[LinkedIn](https://www.linkedin.com/in/mohammadminhaz/) · 📧 minhazurrahman.ds@gmail.com
