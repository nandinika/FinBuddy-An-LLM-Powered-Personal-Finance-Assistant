# FinBuddy-An-LLM-Powered-Personal-Finance-Assistant


## 🚀 Project Overview

**FinBuddy** is a personalized AI-powered financial assistant that provides tailored advice based on users’ transaction histories and financial personas. The system leverages NLP techniques, synthetic transaction generation, and a fine-tuned Qwen model to simulate realistic financial scenarios and deliver actionable insights.  

This repository contains all code, notebooks, and resources to reproduce the project.

---


## 📂 Dataset

This project uses the **Financial Advice Dataset** hosted on [HuggingFace](https://huggingface.co/datasets/Akhil-Theerthala/Kuvera-PersonalFinance-V2.1)  

- **Description:** Contains financial queries, contexts, and advisor-style responses.  
- **Usage:**  
  - Fine-tuning and prompting of Qwen model  
  - Generating synthetic financial personas  
  - Evaluating chatbot personalization  

All preprocessing, cleaning, persona mapping, and synthetic transaction generation is handled in **`notebooks/FinBuddy.ipynb`**.

---

## 📒 Notebooks

### **1️⃣ FinBuddy.ipynb — Full Pipeline**
- Load HuggingFace dataset and persona CSVs  
- Clean, normalize, and preprocess the data  
- Generate realistic synthetic transactions for 5 user personas:
  1. Debt Crisis  
  2. Paycheck-to-Paycheck  
  3. Moderate Saver  
  4. Aggressive Saver  
  5. Overspender  
- Build personalized recommendation pipeline  
- Output qualitative results and evaluation data  

**Location:** `notebooks/FinBuddy.ipynb`

---

### **2️⃣ Chatbot.ipynb — Conversational FinBuddy**
- Implements chatbot functions and transaction analysis  
- Provides persona-aware financial advice  
- Gradio interface for real-time interactions  
- Displays qualitative financial insights per scenario  

**Location:** `notebooks/Chatbot.ipynb`

**Run locally:**
```bash
jupyter notebook notebooks/Chatbot.ipynb
