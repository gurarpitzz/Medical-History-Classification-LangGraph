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
## 🚀 How It Works

1. **Symptom Collection**  
   The user is prompted for their symptoms through an input node.

2. **LLM Classification**  
   The Gemini model is asked to classify the input as one of:
   - `General`
   - `Emergency`
   - `Mental Health`


4. Routing via LangGraph
LangGraph routes the workflow based on LLM output to the appropriate handling node.

5. Final Output
The assistant responds with triage instructions directing the user to the correct hospital department.

---

## 📌 Future Improvements
Add streaming chat interface (e.g., Gradio or Streamlit)

Expand classification categories

Log patient sessions securely

Add multilingual support

---
## 📦 Dependencies

Install all required packages:

```bash
pip install -qU \
    langgraph langchain langchain-core \
    langchain-google-genai \
    google-generativeai==0.8.5 \
    google-ai-generativelanguage==0.6.15
