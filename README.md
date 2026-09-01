# 📚 Academic RAG Assistant: Interactive Textbook & Revision Planner

Transform static educational PDFs into an interactive, personalized AI tutor using Retrieval-Augmented Generation (RAG). 

## 🎯 The Problem
Traditional textbooks suffer from three major educational bottlenecks:
1. **The "One-Size-Fits-All" Delivery:** Textbooks explain concepts in a single, rigid way. If a student doesn't grasp the analogy, they hit a wall.
2. **Study Paralysis:** Dense material often leads to passive reading rather than active learning.
3. **AI Curriculum Drift:** Generic LLMs "hallucinate" or explain concepts using outside terminology that isn't on the student's syllabus.

## 💡 The Solution
This project implements a serverless RAG pipeline that acts as a strict educational guardrail. By utilizing **Google's Gemini 3.6 Flash** and **FAISS Vector Search**, the assistant retrieves exact textbook passages to answer questions accurately, generates active-recall study schedules, and translates complex programming paradigms into highly personalized analogies (e.g., explaining software architecture through tactical midfield positioning).

## ⚙️ Architecture & Tech Stack
* **Core Language:** Python
* **Orchestration:** LangChain (Core & Classic)
* **Embedding Model:** HuggingFace (`all-MiniLM-L6-v2`)
* **Vector Database:** FAISS (Facebook AI Similarity Search)
* **LLM Engine:** Google Gemini (`gemini-3.6-flash`)
* **Environment:** Google Colab / Jupyter Notebooks

## ✨ Core Features
* **Automated Document Ingestion:** Recursively chunks and indexes large technical PDFs (like *The Pragmatic Programmer*) into mathematical vectors.
* **Factual Grounding:** Forces the LLM to answer *only* using retrieved textbook context and cites specific page numbers.
* **Dynamic Personalization:** Modifies the system prompt to explain dense CS concepts using analogies tailored to the user's interests (e.g., football squad management).
* **Active Recall Planner:** Synthesizes retrieved concepts into structured, 3-day revision schedules with challenging self-test questions.

## 🚀 Quick Start (Run on Google Colab)

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/vincemutua/academic-rag-assistant.git]
   cd academic-rag-assistant
