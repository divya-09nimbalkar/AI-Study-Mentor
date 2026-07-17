
```markdown
#  AI Study Mentor

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-2.5--flash-blueviolet.svg)](https://aistudio.google.com/)
[![FAISS](https://img.shields.io/badge/FAISS-Vector_Search-green.svg)](https://faiss.ai)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production_Ready-brightgreen.svg)]()

>  An interactive, personalized study orchestration application that leverages FAISS local vector similarity lookups and Google Gemini 2.5-Flash models to deliver contextual deep explanations, structurally verified MCQ evaluation blocks, and an SQLite-backed spaced repetition scheduling pipeline.

---

##  Table of Contents
- [Overview](#overview)
- [System Architecture](#system-architecture)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Jupyter Cell Execution Pipeline](#jupyter-cell-execution-pipeline)
- [Installation & Environment Setup](#installation--environment-setup)
- [Project Directory Architecture](#project-directory-architecture)
- [License](#license)

---

##  Overview

The AI Study Mentor platform transforms unstructured technical material into a personalized curriculum. By using local dense embeddings via Sentence-Transformers alongside a vectorized database, it extracts targeted reference contexts to dynamically serve multi-tier conceptual tutorials, compile rigorous mock exams, and manage an exponential review schedule.

---

##  System Architecture


Technical Educational Source Material File Input
│
▼
┌──────────────────────────┐
│ Sentence-Transformers    │ ← All-MiniLM-L6-v2 Dense Processing Layouts
└─────────────┬────────────┘
│
▼
┌──────────────────────────┐
│ FAISS Local Index FlatIP │ ← Normal L2 Cosine Vector Similarity Scanners
└─────────────┬────────────┘
│
▼
┌────────────────────────────────────────────────────────┐
│        Gemini 2.5-Flash Processing Pipelines           │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Concept Explainer     │ │ Adaptive MCQ Compiler  │  │
│  └───────────────────────┘ └────────────────────────┘  │
│  ┌───────────────────────┐                             │
│  │ Multi-turn Chatbot    │                             │
│  └───────────────────────┘                             │
└──────────────────────────┬─────────────────────────────┘
│
▼
┌────────────────────────────────────────────────────────┐
│        SQLite Spaced Repetition Retention Engine       │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ SM-2 Interval Log     │ │ Matplotlib Dashboard   │  │
│  └───────────────────────┘ └────────────────────────┘  │
└────────────────────────────────────────────────────────┘

```

---

##  Key Features

* **Local RAG Embedding Architectures:** Uses `Sentence-Transformers` to encode text variables locally, searching database logs via an internal FAISS flat index vector store.
* **Structurally Enforced MCQ Matrices:** Leverages Gemini `response_mime_type` bindings to compile parseable multiple-choice evaluation JSON items without data leakage risks.
* **SQLite Persistence Layer:** Tracks session timelines, calculates historical error logs, and automatically runs memory retention parameters across specific concepts.
* **Multi-Turn Mentoring Agent:** Maintainable conversation session cache built to surface architectural system comparisons smoothly.
* **Matplotlib Strategy Maps:** Automatically tracks user profile mastery thresholds, grouping results into horizontal bar charts saved to `output/`.

---

##  Tech Stack

* **AI Reasoning Framework:** Google Gemini 2.5-Flash (`google-generativeai`)
* **Vector Vector Store Index:** Facebook AI Similarity Search (`faiss-cpu`)
* **Sentence Embeddings Mapping:** HuggingFace `sentence-transformers` (`all-MiniLM-L6-v2`)
* **Relational Database Memory:** SQLite3 Database Engine
* **Visual Representation Interface:** Matplotlib Graphing Engine
* **Application UI Container:** Gradio Blocks Framework (Gradio 6.0+ compatible)

---

##  Jupyter Cell Sequence Blueprint

The `AI_Study_Mentor.ipynb` notebook workspace follows a linear, 9-cell structure:

| Cell # | Type | Target Module Context | Technical Core Purpose |
| :--- | :--- | :--- | :--- |
| **Cell 1** |  Markdown | **Project Introduction** | System summary badges, feature indices, and blueprint architectures. |
| **Cell 2** |  Code | **Package Downloads** | Silent environment hydrations (`%pip install`) of FAISS, GenAI, and UI frameworks. |
| **Cell 3** |  Code | **Global Initializations** | Standard imports, environment keys configurations, and core structural data classes. |
| **Cell 4** |  Code | **RAG Knowledge Base** | Implements `KnowledgeBase` vector mapping pipelines via local FAISS configurations. |
| **Cell 5** |  Code | **Adaptive MCQ Generator** | Drives `QuizGenerator` managing json evaluation items and CLI question iterations. |
| **Cell 6** |  Code | **SQLite Metrics Log** | Runs `ProgressTracker` handling spaced repetition dates loops and plotting functions. |
| **Cell 7** |  Code | **Mentor Core Agent** | Groups system parts under `AIStudyMentor` handling multi-turn study sessions. |
| **Cell 8** |  Code | **Verification Run** | Validates the full framework stack using a robust try-except quota isolation architecture. |
| **Cell 9** |  Code | **Gradio Interface App** | Mounts individual tab interfaces for concept evaluations directly inside browser displays. |

---

##  Installation & Environment Setup

### 1. Build Local Target Project Workspace
```bash

cd AI_Study_Mentor
python -m venv venv
source venv/bin/activate # Windows Terminal: .\venv\Scripts\activate

```

### 2. Deploy Dependencies Manifest

```bash
pip install -r requirements.txt

```

### 3. Setup Gemini Access Token

Register for a free API access key directly at [Google AI Studio](https://aistudio.google.com/). Paste your secret key parameter inside **Cell 3** of your notebook configuration file:

```python
os.environ["GEMINI_API_KEY"] = "AIzaSyYourSecretKeyStringHere"

```

---

##  Project Directory Architecture

```text
AI_Study_Mentor/
├── notebooks/
│   └── AI_Study_Mentor.ipynb      # Main interactive development notebook workspace
├── output/
├── .gitignore                     # Git configuration element tracking blocks
├── README.md                      # Comprehensive system documentation (This file)
└── requirements.txt               # Pinned application dependencies manifest

```

---

##  Author

**Divya** — AI/ML Developer | B.Tech Electronics & Telecom


