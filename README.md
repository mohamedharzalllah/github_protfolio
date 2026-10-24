<div align="center">

# Mohamed Harzallah

**AI Engineer · Generative AI, LLM agents & Data Science**

Computer engineer · M2 in Artificial Intelligence & Data Science, Université Paris-Dauphine (Tunis campus), graduating Dec. 2026

[🌐 Portfolio website](https://mohamedharzalllah.github.io/github_protfolio/) ·
[📄 CV](cv/Mohamed_Harzallah_CV.pdf) ·
[💼 LinkedIn](LINKEDIN_URL) ·
[✉️ Email](mailto:EMAIL_ADDRESS) ·
[🐙 GitHub](https://github.com/mohamedharzalllah)

</div>

---

## About me

I build AI systems that go from raw, messy data to answers people can use: multi-agent LLM pipelines that combine document retrieval (RAG) with structured SQL data, natural-language interfaces over databases, and deep learning models for medical imaging. I care about evaluation as much as modelling. Several projects below include test suites, reference checks or controlled comparisons, and their READMEs state known limitations openly.

I currently work on **IRIS Agent** at IRIS IT, a multi-agent LLM document-intelligence platform for health-insurance brokerage. I am open to **AI / GenAI engineering roles** (remote-friendly) and research positions in agentic AI.

**Languages:** French (C1) · English (B2)

---

## Skills

| Area | Tools |
|---|---|
| **GenAI & LLM agents** | LangChain, LangGraph, RAG, Gemini API, prompt engineering, LLM-as-judge evaluation, Sentence-BERT |
| **Machine & deep learning** | PyTorch, TensorFlow/Keras, scikit-learn, XGBoost / LightGBM / CatBoost, YOLOv8, Faster R-CNN, contrastive / self-supervised learning |
| **Data engineering & big data** | Apache Spark (PySpark, Scala), Kafka, Spark Structured Streaming, DuckDB, SQL |
| **Databases** | MongoDB, Neo4j, Redis, HBase, RDF/SPARQL (Jena Fuseki), FAISS / Chroma vector stores |
| **Cloud & deployment** | Google Cloud (BigQuery, Cloud Storage), Docker / Docker Compose, FastAPI, Streamlit |
| **Optimisation** | Google OR-Tools (CVRP / MDVRP), K-Means clustering, heuristics |

---

## Featured projects

### 🤖 Generative AI & LLM agents

| Project | What it does | Stack |
|---|---|---|
| **IRIS Agent** · *professional, private code* | Multi-agent LLM platform for document management and intelligence in health-insurance brokerage, built at IRIS IT. Subject of my M2 internship report. | LLM agents, document AI |
| [**telecom-agent**](https://github.com/mohamedharzalllah/telecom-agent) | Multi-agent customer-support assistant for a fictional telecom operator. A LangGraph router sends each question to a **RAG** branch (FAQ PDFs), a **SQL** branch (customer, billing and consumption tables) or a **hybrid** branch, and a judge agent checks the answer. Ships with an evaluation script and a Streamlit demo. | LangGraph, Gemini 2.5 Flash, FAISS, DuckDB, Streamlit |
| [**advanced_database** · NoSQL-LLM](https://github.com/mohamedharzalllah/advanced_database) | Natural-language querying across **5 NoSQL databases**: an LLM translates plain-English questions into MongoDB, Cypher, Redis, HBase and SPARQL queries, validates them and compares results across databases. Includes a CLI and a web UI. | Gemini, MongoDB, Neo4j, Redis, HBase, Jena Fuseki, Docker Compose |
| [**cv-job-graph-matching**](https://github.com/mohamedharzalllah/cv-job-graph-matching) | CV ↔ job-offer matching as a bipartite graph, enriched with Sentence-BERT semantic similarity. Covers Louvain communities, Adamic-Adar link prediction and seniority classification from embeddings plus graph features. *With G. Nader.* | NetworkX, Sentence-BERT, scikit-learn |
| [**hybrid-fd-discovery**](https://github.com/mohamedharzalllah/hybrid-fd-discovery) | Data-quality pipeline that discovers functional dependencies with **TANE** and **FastFD** (both implemented from scratch), flags suspicious ones and prepares them for LLM review. Both algorithms agree on 8 UCI datasets and match a brute-force reference. | Python, CLI, tests |

### 🩻 Computer vision & medical imaging

| Project | What it does | Stack |
|---|---|---|
| [**Fusion-multimodale-imagerie**](https://github.com/mohamedharzalllah/Fusion-multimodale-imagerie) | Multimodal self-supervised learning that combines mammography images with clinical tabular data. Simplified re-implementation of Hager et al., CVPR 2023, with an FT-Transformer tabular encoder, per-column missing-value embeddings and a controlled 7-method comparison. | PyTorch, InfoNCE, FT-Transformer |
| [**Breast density, ordinal regression**](https://github.com/mohamedharzalllah/Estimation-de-la-densit-mammaire-en-r-gression-ordinale) | BI-RADS breast-density classifier (A–D) on VinDr-Mammo trained with an ordinal-aware **CORN** loss, compared with cross-entropy and evaluated with Quadratic Weighted Kappa. Handles DICOM pitfalls (MONOCHROME1, VOI LUT) and patient-level splits. | PyTorch, DICOM, ordinal regression |
| [**chest-xray-pathology-detection**](https://github.com/mohamedharzalllah/chest-xray-pathology-detection) | Detection of 8 thoracic pathologies on NIH ChestX-ray14 using **YOLOv8-L** and **Faster R-CNN** with CLAHE, small anchors and box fusion (NMS / WBF). | Ultralytics YOLOv8, torchvision, Kaggle GPU |
| [**alzheimer-detection**](https://github.com/mohamedharzalllah/alzheimer-detection) | Alzheimer detection from 450 handwriting features (Kaggle competition). Compares a PCA + stacking ensemble (XGBoost, LightGBM, CatBoost, SVM…) with a residual MLP trained with focal loss and L1 feature selection. | scikit-learn, TensorFlow, XGBoost |

### 📝 NLP

| Project | What it does | Stack |
|---|---|---|
| [**cnn-dailymail-summarization**](https://github.com/mohamedharzalllah/cnn-dailymail-summarization) | News summarisation on CNN/DailyMail: TF-IDF extractive vs LSTM seq2seq vs seq2seq with **Bahdanau attention**, scored with ROUGE-1/2/L. *With S. A. Afi.* | TensorFlow/Keras, ROUGE |

### ⚙️ Data engineering, big data & cloud

| Project | What it does | Stack |
|---|---|---|
| [**data-streaming-project**](https://github.com/mohamedharzalllah/data-streaming-project) | Real-time weather pipeline: OpenWeather → Kafka → Spark Structured Streaming with Random Forest temperature prediction and Isolation Forest anomaly detection → live dashboard. Fully dockerised. | Kafka, PySpark, scikit-learn, Streamlit, Docker |
| [**GCP_movie_recommendation_project**](https://github.com/mohamedharzalllah/GCP_movie_recommendation_project) | End-to-end movie recommender on Google Cloud: BigQuery → GCS ingestion, data validation, cold-start handling, model training and a FastAPI + Streamlit serving layer. | BigQuery, GCS, FastAPI, Streamlit |
| [**ccf-connected-components-spark**](https://github.com/mohamedharzalllah/ccf-connected-components-spark) | Connected components with the CCF MapReduce algorithm (Kardes et al., 2014), implemented with RDD and DataFrame APIs in **Scala and PySpark** and benchmarked. | Spark, Scala, PySpark |

### 🚚 Optimisation

| Project | What it does | Stack |
|---|---|---|
| [**Advanced Multi-Depot VRP**](https://github.com/mohamedharzalllah/Advanced-Multi-Depot-VRP-Optimization-System) | Delivery optimisation (CVRP → multi-depot VRP) with OR-Tools: K-Means clustering, baselines, dynamic re-optimisation with rolling horizon, and cost / CO₂ business metrics across scenarios, plus an interactive dashboard. | OR-Tools, K-Means, Streamlit |

---

## Education

- **M2 Artificial Intelligence & Data Science**, Université Paris-Dauphine, Tunis campus (expected December 2026)
- **Computer Engineering degree**, Faculté des Sciences de Tunis
- Two years of preparatory classes (classes préparatoires)

---

<div align="center">
<sub>This repository hosts my portfolio. The website is served from <code>index.html</code> via GitHub Pages.</sub>
</div>
