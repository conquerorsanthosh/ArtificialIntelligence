# Artificial Intelligence — Applied Coursework & Projects

Hands-on work from the **Master of Applied Artificial Intelligence (Global)**, Deakin University (Oct 2025 – Oct 2027).

This repository holds working notebooks rather than exercises — each folder is a complete project with a problem statement, data, modelling, and evaluation. My background is 21+ years in distributed systems and platform engineering; this is where I build the AI side of that.

**Santhosh Krishnamurthy** · [LinkedIn](https://www.linkedin.com/in/sankrishms/)

---

## Projects

### `AgenticAI/` — NewsFindR
A personalised news-retrieval agent built as a **ReAct agent on LangGraph**.

- **SQL agent toolkit** over a SQLite database of user interests, so the agent queries for what a given user cares about rather than being told
- **Web search as a callable tool** (DuckDuckGo) for real-time retrieval
- **Credibility filtering** to screen sources before summarisation
- **Pydantic-structured outputs** for predictable downstream handling
- **Groq** for inference, with token-per-minute rate limiting

*Stack: LangGraph, LangChain, ChatGroq, SQLDatabaseToolkit, DDGS, Pydantic, SQLite*

---

### `RAG/` — Medical Assistant
A retrieval-augmented generation pipeline over medical manuals and research papers, built to give clinicians fast access to trustworthy source material.

- **PDF ingestion** with PyMuPDF
- **Recursive chunking** tuned for dense technical documents
- **Sentence-transformer embeddings** and a **Chroma** vector store
- **Local Llama inference** via llama.cpp — no external API dependency

*Stack: LangChain, Chroma, HuggingFace embeddings, PyMuPDF, llama.cpp, tiktoken*

---

### `Model Deployment/` — SuperKart
Retail sales forecasting, taken end to end from notebook to deployed service.

- Feature engineering and **scikit-learn pipelines** with column transformers
- **XGBoost regressor**, tuned with GridSearchCV
- Model serialised with joblib, served through a **Flask API**
- **Containerized with Docker** and deployed to **Hugging Face**
- **Streamlit** front end for interactive prediction

*Stack: scikit-learn, XGBoost, Flask, Docker, Hugging Face Hub, Streamlit, joblib*

---

### `Bagging-Boosting/` — EasyVisa
Binary classification predicting US visa certification outcomes, comparing ensemble methods on an imbalanced dataset.

- Decision trees, random forest, **bagging, AdaBoost, gradient boosting, XGBoost**
- **SMOTE oversampling and random undersampling** to handle class imbalance
- Hyperparameter tuning with RandomizedSearchCV
- Model comparison on recall-weighted metrics, since false negatives carry the cost here

*Stack: scikit-learn, XGBoost, imbalanced-learn, pandas, seaborn*

---

### Other folders

| Folder | Contents |
|---|---|
| `Neural Networks/` | Feedforward networks, optimisation and tuning |
| `Computer Vision/` | Image processing and convolutional neural networks |
| `DecisionTree/` | Tree-based classification and interpretability |
| `MLOps/` | ML pipelines, DevOps for ML, model interpretability |
| `Statistics/` | Inferential statistics, hypothesis testing, EDA |
| `Introduction To Python/` | Data manipulation, exploratory data analysis |

---

## Also covered

Transformers and attention mechanisms · embeddings · prompt engineering · **LLM fine-tuning with QLoRA** · model interpretability · containerization

---

## Notes

Notebooks were developed in Google Colab; paths reference Drive mounts in places. Datasets are course-provided and not redistributed here.
