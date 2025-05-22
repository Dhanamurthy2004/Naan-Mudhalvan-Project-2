# Naan-Mudhalvan-Project-2

# 🧠 PDF Summarizer & Chatbot with RAG + LLM Integration

This project is a **Streamlit web app** that leverages **LangChain**, **LLMs (LLaMA3/Groq)**, and **RAG (Retrieval-Augmented Generation)** to provide two powerful capabilities:

* 📄 **PDF Summarization** – Generate short and long summaries of uploaded PDFs using LLMs.
* 💬 **PDF Q\&A Chatbot** – Chat with your PDF using a RAG-powered chatbot that retrieves relevant chunks and answers questions contextually.

---

## 🚀 Features

### ✅ PDF Summarization (Two Modes)

* Upload a PDF.
* Generates:

  * 🔹 A concise summary (\~100 words).
  * 🔹 A detailed summary (\~1000 words).
* Uses the **Groq LLaMA3-8B** or **LLaMA3-70B** model.

### ✅ Chat with Your Documents

* Upload another PDF to create a knowledge base.
* Chat directly with the content using a chatbot powered by:

  * **LangChain Retriever + Vector DB (FAISS)**
  * **HuggingFace / Google Embeddings**
  * Contextual memory for follow-up questions.

### ✅ Beautiful UI

* Custom styled using advanced CSS in Streamlit for an enhanced experience.
* Clear sections for summarization and Q\&A.

---

## 🧰 Tech Stack

| Component          | Technology                                  |
| ------------------ | ------------------------------------------- |
| 💬 LLM             | Groq's LLaMA3-8B / 70B via `langchain_groq` |
| 🧠 Embeddings      | HuggingFace & Google Generative AI          |
| 📄 PDF Handling    | `PyMuPDFLoader`, `PyPDF2`                   |
| 🔍 RAG & Vector DB | FAISS + LangChain Retriever Pipeline        |
| 🌐 Frontend        | Streamlit with custom CSS                   |

---

## 📁 File Structure

```bash
📦 NM-Project
├── fulrag.py       # Main app with summarization and chatbot features
├── part1.py        # Alternative or minimal version of the app
├── README.md       # This file
```

---

## 🧪 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/nm-project-rag.git
cd nm-project-rag
```

### 2. Install Requirements

Create a virtual environment and install dependencies:

```bash
pip install -r requirements.txt
```

If `requirements.txt` doesn't exist, create one with:

```txt
streamlit
langchain
langchain-community
langchain-core
langchain-groq
langchain-huggingface
langchain-google-genai
sentence-transformers
PyPDF2
PyMuPDF
faiss-cpu
```

### 3. Set Environment Variables

Create a `.env` file:

```env
GOOGLE_API_KEY=your_google_api_key
```

> You’ll be asked to enter your **Groq API key** in the Streamlit sidebar.

---

## 🏃 Running the App

```bash
streamlit run fulrag.py
```

* Visit `http://localhost:8501` in your browser.
* Upload a PDF to summarize and chat.

---

## 📸 Screenshots

| Summarizer Section                          | Chatbot Section                       |
| ------------------------------------------- | ------------------------------------- |
| ![Summarizer](./screenshots/summarizer.png) | ![Chatbot](./screenshots/chatbot.png) |

---

## ⚙️ Future Enhancements

* ☑️ Multi-file knowledge base
* ☑️ Caching and faster vector search
* ☑️ Support for other formats (DOCX, TXT)
* ☑️ Feedback-based improvement loop

---

## 🤝 Acknowledgements

* [LangChain](https://www.langchain.com/)
* [Groq API](https://console.groq.com/)
* [Streamlit](https://streamlit.io/)
* [HuggingFace Transformers](https://huggingface.co/)

---

## 👤 Author
Developed by Dhanamurthy P

Jeppiaar Engineering College – Department of Artificial Intelligence and Data Science

## 📜 License

MIT License – Feel free to fork, customize, and contribute!

