## 🚀 Hire-Er-Key (GenAI Engineer Edition)

Hire-Er-Key (pronounced *Hierarchy*) is a RAG-based AI system designed to intelligently match candidates to job descriptions using hybrid retrieval, structured scoring, and LLM-based reasoning.

---

## 🔹 Features

* 🔍 Hybrid Retrieval (FAISS + BM25)
* 🧠 Skill-based weighted scoring (Must-Have / Important / Nice-to-Have / Implicit)
* ⚖️ Comparative ranking using LLM (WhosBetter)
* 📊 Explainable outputs (Strengths & Gaps)
* 🤖 Agent Dispatcher (Hero)
* 🎯 Confidence scoring
* 🧾 Clean structured output

---

## 🧠 System Architecture

```
Resumes → Metadata Extraction → FAISS DB
        → Job Description Parsing
        → Hybrid Retrieval
        → Skill Matching
        → Ranking
        → Explanation
```

---

## ⚙️ How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

---

### 2. Run Notebook

Open:

```
notebook/hire_er_key.ipynb
```

Run all cells sequentially.

---

### 3. Run UI (Demo Mode)

```bash
python app/gradio_app.py
```

---

## 🎯 Output

For each candidate:

* Final Fit Score
* Rank
* Strengths
* Skill Gaps
* Confidence Level

---

## 🚀 Versioning

### ✅ V1.0

* Core RAG pipeline
* Hybrid retrieval
* Scoring + explanation
* Dispatcher (Hero)

---

### 🚀 V2.0 (Minimal Enhancements)

* Top-K candidate selection
* Candidate name extraction
* Improved output formatting

---

### 🔮 V3.0 (Future Scope)

* Dynamic Job Description support
* Semantic skill equivalence using LLM
* Role-based dynamic thresholding
* Alternate job role recommendations for rejected candidates
* Latency optimization (batching / async)
* Enhanced UI/UX

---

## ⚠️ Demo Note

Due to API rate limits, metadata extraction and scoring are precomputed for demonstration.
The system supports full dynamic execution in production settings.

---

## 🧠 Key Insight

Hire-Er-Key is not just a retrieval system, but a **multi-stage AI decision pipeline** combining:

* Retrieval
* Structured evaluation
* LLM reasoning
* Explainability

