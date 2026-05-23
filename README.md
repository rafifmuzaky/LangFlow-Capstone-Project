# Employee Self Service Assistant

## Description

Employee Self Service Assistant is an AI-based chatbot designed to help employees access internal company information quickly and efficiently. The system uses Retrieval-Augmented Generation (RAG) technology to answer user questions based on company documents such as employee handbooks, SOPs, HR policies, and other internal files.

This project integrates Google Generative AI Embeddings, Astra DB as a vector database, and Large Language Models (LLM) to provide accurate and contextual responses.

---

# Features

* AI chatbot for internal company information
* Retrieval-Augmented Generation (RAG)
* Company document search using vector embeddings
* Fast and contextual responses
* Astra DB integration for vector storage
* Support for employee handbook and HR policy documents

---

# Technologies Used

* Python
* Langflow
* Astra DB
* Google Generative AI Embeddings
* Gemini / LLM
* Retrieval-Augmented Generation (RAG)

---

# System Workflow

## Input

User enters a question through the chatbot interface.

## Process

1. User question is converted into embeddings.
2. Astra DB searches for relevant company documents.
3. Retrieved documents are processed through a prompt template.
4. LLM generates answers based on retrieved context.

## Output

The chatbot provides accurate answers based on company documents.

---

# Project Architecture

```text id="wkjlq9"
PDF Documents
      ↓
Text Splitter
      ↓
Embedding Model
      ↓
Astra DB Vector Store
      ↓
Retriever
      ↓
Prompt Template
      ↓
LLM (Gemini)
      ↓
Chatbot Response
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/rafifmuzaky/Employee-Self-Service-Assistant.git
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Configuration

Configure the following environment variables:

```env
ASTRA_DB_API_ENDPOINT=your_astra_endpoint
ASTRA_DB_APPLICATION_TOKEN=your_token
GOOGLE_API_KEY=your_google_api_key
```

---

# Running the Project

```bash
python app.py
```

or run the flow directly using Langflow.

---

# Example Questions

* What is the company leave policy?
* How many annual leave days are available?
* What are the employee working hours?
* Explain the company SOP for remote work.

---

# Future Development

* Multi-user authentication
* Voice assistant integration
* HR system integration
* Employee onboarding assistant
* Mobile application support
* Conversation memory feature

---

# Author

Muhammad Rafif Muzaky

---

# License

This project is developed for educational and capstone project purposes.
