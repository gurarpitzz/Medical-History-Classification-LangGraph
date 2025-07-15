# 🏥 Dr. Singh Hospital – AI Symptom Classifier using LangGraph & Gemini

Welcome to the repository for **Dr. Singh Hospital**, an AI-powered medical assistant that classifies patient symptoms into **General**, **Emergency**, or **Mental Health** categories using Google's **Gemini 1.5 Flash** model and a graph-based reasoning system via **LangGraph**.

---

## 🧠 Overview

This project simulates a hospital triage assistant that:
- Prompts the user for symptoms
- Classifies symptoms using LLM-based reasoning
- Routes the patient to the correct medical department

It demonstrates:
- Use of **LangGraph** to build modular, stateful workflows
- Integration with **Gemini** via `langchain-google-genai`
- Graph-based logic with **conditional branching**

---

## 📦 Dependencies

Install all required packages:

```bash
pip install -qU \
    langgraph langchain langchain-core \
    langchain-google-genai \
    google-generativeai==0.8.5 \
    google-ai-generativelanguage==0.6.15
