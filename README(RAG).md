
# Task 2 – Analytical Chatbot (RAG & Explanation)

## 📌 Brief Task Description
This project implements an **Analytical Chatbot** that allows users to ask natural language questions about stock market movements.
The system identifies relevant stock tickers, analyzes recent price trends, retrieves contextual financial news, and explains market behavior using a **Retrieval-Augmented Generation (RAG)** approach.

This is an **individual task submission**, completed according to the provided instructions.

---

## 🎯 Objective
- Answer queries such as:
  - “Why did Apple stock drop?”
  - “When did Microsoft go up?”
- Identify the correct stock ticker from the query
- Analyze short-term stock price trends
- Retrieve relevant financial news articles
- Generate clear, human-readable explanations

---

## 🧠 Approach & Architecture
The solution follows a **modular, agent-based design**:

1. **Intent Understanding**
   - Interprets the user’s natural language query

2. **Research (Retrieval)**
   - Fetches recent financial news
   - Stores text embeddings in a vector database

3. **Trend Analysis**
   - Analyzes recent historical stock prices

4. **Explanation Generation**
   - Combines retrieved news and trends
   - Uses an LLM to generate explanations

The workflow is orchestrated using **LangChain’s RunnableSequence (LCEL)**.

---

## 🧰 Tech Stack
- Python
- Groq API (LLM – LLaMA 3.1)
- NewsAPI (financial news retrieval)
- yfinance (stock price data)
- SentenceTransformers (embeddings)
- FAISS (vector similarity search)
- LangChain (RunnableSequence)

---

## ▶️ Instructions to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone <your-github-repo-url>
cd task-2-analytical-chatbot
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Add API Keys (Locally or in Google Colab)
⚠️ **Do NOT hardcode or commit API keys to this repository.**

Use placeholders in code and set real keys only in your local environment or Colab:
```python
GROQ_API_KEY = "your_groq_api_key"
NEWS_API_KEY = "your_newsapi_key"
```

### 4️⃣ Run the Notebook
- Open the notebook in **Google Colab**
- Run all cells sequentially
- Example usage:
```python
analytical_chatbot("Why did Apple stock drop?")
```

---

## 📸 Related Screenshots
Add screenshots showing:
- Successful execution in Google Colab
- Example chatbot responses

---

## 🌐 Hosted URL
Not hosted.

---

## 🔐 Security Note
- This repository **does NOT contain any real API keys or secrets**.
- All sensitive credentials must be provided locally and never committed to version control.

---

## ⚠️ Notes
- This is an **individual task submission** (no collaboration).
- The task is **self-contained** and represents one valid interpretation.
- Code is submitted even if incomplete, as per instructions.
- Emphasis is on **clarity, structure, and correct application of concepts**.

---

## 👤 Author
Individual submission for **Task 2 – Analytical Chatbot (RAG & Explanation)**.
