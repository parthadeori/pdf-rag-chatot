# 📄 PDF RAG Chatbot

A **Retrieval-Augmented Generation (RAG)** chatbot that allows users to upload a PDF and ask questions about its content.  
The system retrieves relevant document chunks from a vector database and generates answers using an LLM.

Built using **LangChain, Chroma, Groq, and Streamlit**.

---

## 🚀 Features

- Upload any PDF document
- Automatically split documents into chunks
- Generate embeddings using HuggingFace models
- Store embeddings in **Chroma vector database**
- Retrieve relevant context for user queries
- Generate answers using **Groq LLM**
- Simple interactive **Streamlit UI**

---

## 🧠 Architecture

```

User Question
↓
Streamlit UI
↓
LangChain Retriever
↓
Chroma Vector Database
↓
Relevant Document Chunks
↓
Groq LLM
↓
Generated Answer

```

---

## 🛠️ Tech Stack

- **Python**
- **Streamlit** – Web interface
- **LangChain** – LLM orchestration
- **ChromaDB** – Vector database
- **HuggingFace Embeddings**
- **Groq API** – LLM inference
- **PyPDF** – PDF document loading

---

## 📂 Project Structure

```

pdf-rag-chatbot
│
├── app.py
├── rag_pipeline.py
├── requirements.txt
├── README.md
├── .gitignore
└── .env (not included in repo)

```

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```

git clone [https://github.com/parthadeori/pdf-rag-chatbot.git](https://github.com/parthadeori/pdf-rag-chatbot.git)
cd pdf-rag-chatbot

```

---

### 2️⃣ Create virtual environment

```

python -m venv venv

```

Activate it:

Windows

```

venv\Scripts\activate

```

Mac/Linux

```

source venv/bin/activate

```

---

### 3️⃣ Install dependencies

```

pip install -r requirements.txt

```

---

### 4️⃣ Set up environment variables

Create a `.env` file:

```

GROQ_API_KEY=your_api_key_here

```

---

### 5️⃣ Run the application

```

streamlit run app.py

```

---

## 💡 Example Usage

1. Upload a PDF document
2. Ask a question about the document
3. The system retrieves relevant context and generates an answer

Example question:

```

What is machine learning?

```

---

## 🔒 Security Note

API keys are stored in `.env` and **excluded from GitHub using `.gitignore`**.

---

## 📈 Future Improvements

- Chat-style interface
- Persistent vector database
- Multi-document support
- Deployment on Streamlit Cloud / HuggingFace Spaces

---

## 👨‍💻 Author

**Partha Deori**

GitHub:  
https://github.com/parthadeori

---
