# 📘 PDF Intelligence System with Retrieval Augmented Generation (RAG)


## 📌 Overview
The **PDF Intelligence System** is a user-centric and intelligent platform that enhances information retrieval from PDF documents using **natural language queries**.  
By leveraging **Retrieval Augmented Generation (RAG)**, the system enables users to interact with PDF content in a seamless and intuitive manner, eliminating the need for manual search.  

This project integrates **FAISS**, **Hugging Face embeddings**, **OpenAI GPT-3.5 Turbo**, and **Streamlit UI** to deliver an adaptive and reliable document querying experience.

---

## 🔍 Retrieval Augmented Generation (RAG)

### Introduction
**RAG** (introduced by Meta AI) is designed for knowledge-intensive tasks. It combines:
- **Information Retrieval** → Finds relevant context from documents.  
- **Text Generation** → Uses LLMs to produce coherent and accurate responses.  

Unlike traditional models that require retraining for every knowledge update, RAG allows **dynamic retrieval** without retraining the core LLM.

---

## ⚙️ Workflow
1. **Input** → Users upload multiple PDF files.  
2. **VectorStore** → PDFs are converted into vector representations using **FAISS** and **all-MiniLM-L6-v2** embeddings from Hugging Face.  
3. **Memory** → A **conversation buffer memory** tracks the dialogue and feeds context to the model.  
4. **Text Generation** → Queries and retrieved context are passed to **GPT-3.5 Turbo (OpenAI API)** for generating responses.  
5. **User Interface** → Built with **Streamlit** for simplicity and interactivity.  

---

## 🎯 Benefits
- **Adaptability** → Updates with evolving knowledge domains.  
- **Efficiency** → Combines retrieval + generation for real-time knowledge access.  
- **Reliability** → Produces factually grounded outputs by blending search with generation.  

---

## 🚀 Project Features
- 🖥️ **User-Friendly Interface** → Ask questions in natural language.  
- 📑 **Multi-PDF Support** → Upload and query multiple documents.  
- ⚡ **Seamless Navigation** → Quick retrieval with conversational context.  
- 🔁 **Conversational Memory** → Keeps track of previous queries for continuity.  

---

## 🛠️ Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/rutikakengal/ChatPDF.git
cd ChatPDF
```
2️⃣ Install Dependencies
```
pip install -r requirements.txt
```

3️⃣ Run the Application
```
streamlit run app.py
```

4️⃣ Open in Browser
Navigate to:
👉 http://localhost:8000


🤝 Contributing

We welcome contributions to enhance the PDF Intelligence System 🎉
Please read our Contribution Guidelines
 before submitting PRs.

 ---

 ## 🙏 Acknowledgments

Hugging Face → For the all-MiniLM-L6-v2 embeddings model.

OpenAI → For providing GPT-3.5 Turbo API.

Meta AI → For introducing the RAG methodology.
