# 🎓 Academic Research Assistant (AI for Scholars)
> **AI-Powered Paper Summarization + Citation-Based Q&A System**

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-orange.svg)
![LangChain](https://img.shields.io/badge/Framework-LangChain-green.svg)
![ChromaDB](https://img.shields.io/badge/Database-ChromaDB-purple.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

---

## 🧩 Problem Statement

**Problem #10: Academic Research Assistant (Paper Summarization + Citation Q&A)**  
Build a system that automatically **summarizes research papers** and enables **question-answering with source citations**.  

- **Dataset:** [Kaggle – ArXiv Academic Papers Dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv)  
- **Outcome:** Vectorized paper index + RAG retrieval for topic-based Q&A + Markdown summaries  
- **Stack:** `Python`, `LangChain`, `Embeddings`, `ChromaDB`, `LLM API`, `Streamlit`

---

## 📘 Overview

**AI for Scholars** is a next-generation **AI-powered Academic Research Assistant** that helps researchers, clinicians, and students synthesize multiple academic papers into actionable insights.

The system:
- 🧠 Summarizes uploaded papers into structured markdown reports  
- 🧾 Builds **vectorized embeddings** for semantic search  
- 💬 Enables **retrieval-augmented Q&A** with **citation references**  
- 🕸️ Constructs **knowledge graphs** to reveal conceptual relationships  
- 🗣️ Generates **audio summaries** for accessibility  

It combines **LangChain’s RAG pipeline**, **ChromaDB vector store**, and **local/remote LLM APIs** for intelligent, explainable research assistance.

---

## ⚙️ Core Features

| Feature | Description |
|----------|-------------|
| 📄 **PDF Ingestion & Cleaning** | Extracts text via pdfplumber (PyPDF2 fallback) and cleans metadata |
| 🧬 **Concept & Entity Extraction** | Uses spaCy, regex, and TF-IDF for biomedical entity detection |
| 🔗 **Knowledge Graph Visualization** | Constructs explainable graphs using NetworkX + Plotly |
| ⚖️ **Contradiction Detection** | Finds cross-paper contradictions via semantic/sentiment analysis |
| 💡 **Research Gap Finder** | Highlights underexplored research areas with impact scoring |
| 🧠 **Vector Indexing (RAG)** | Embeds and stores research chunks in **ChromaDB** for retrieval |
| 🧾 **Summarization Engine** | Creates concise Markdown-based paper summaries |
| 💬 **Citation-based Q&A** | Answers queries with citation-linked references using LangChain |
| 🔊 **Audio Summarization** | Converts text results to audio using pyttsx3 or Groq/gTTS |
| 🧰 **Configurable Streamlit UI** | Real-time sliders, visualization, and export options |
| 🔒 **Local-First Architecture** | Works fully offline; integrates Ollama, Groq, Gemini optionally |

---

## 🧠 System Architecture

The following architecture illustrates the **complete AI-powered academic research assistant pipeline**, connecting all the major modules, databases, and user interfaces.

<p align="center">
  <img src="assets/system_architecture.png" alt="System Architecture Diagram" width="800"/>
</p>

**Architecture Summary:**
1. **User Uploads PDFs** → The system ingests and normalizes text.
2. **Concept Extraction Layer** → Detects medical/academic entities using NLP and TF-IDF.
3. **Knowledge Graph Builder** → Maps relationships and contradictions between extracted concepts.
4. **Vector Indexing (ChromaDB)** → Creates embeddings for each chunk of paper data.
5. **RAG Retrieval Engine (LangChain)** → Handles question-answering with citation references.
6. **Streamlit Frontend** → Displays interactive dashboards, graphs, Q&A, and audio summaries.
7. **Audio Synthesizer** → Converts summaries into speech (WAV/MP3 format).

---

## 🔄 Data Flow Diagram

The following diagram shows the data movement through each stage of the system, from upload to retrieval and output.

<p align="center">
  <img src="assets/data_flow_diagram.png" alt="Data Flow Diagram" width="800"/>
</p>

**Flow Explanation:**
1. **PDF Upload:** User uploads multiple research papers.  
2. **Extraction:** The system extracts, cleans, and segments the text.  
3. **Summarization:** A markdown summary is generated for each paper.  
4. **Embedding & Storage:** The papers are vectorized and stored in ChromaDB.  
5. **Retrieval (RAG):** On queries, the most relevant chunks are retrieved.  
6. **Citation Q&A:** LangChain generates contextual answers with citation links.  
7. **Visualization:** Insights are represented as graphs, treemaps, and mind maps.  
8. **Audio Summary:** Results are converted into an audio briefing for accessibility.  


