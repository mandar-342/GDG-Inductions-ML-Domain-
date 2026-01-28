
# Task 2 – Analytical Chatbot (RAG & Explanation)

## 📌 Brief Task Description
This task involves building an analytical chatbot that allows users to ask natural language questions about stock market movements. The system identifies relevant stock tickers from the query, analyzes recent price trends, and retrieves related financial news to provide contextual understanding of market behavior.

The chatbot follows a Retrieval-Augmented Generation (RAG) approach, where external information is retrieved and combined with an LLM to generate clear explanations. A modular, agent-based architecture is used to separate intent understanding, news retrieval, trend analysis, and explanation generation. This task highlights the application of RAG, LLMs, and structured reasoning to explain real-world data.

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

## 🔐 Security Note
- This repository **does NOT contain any real API keys or secrets**.
- All sensitive credentials must be provided locally and never committed to version control.


