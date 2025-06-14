# 🧠 COVID-19 & Smoking QnA Agent (CORD-19 NLP Project)

This project explores the relationship between **smoking** and **COVID-19** using machine learning and natural language processing techniques applied to the **CORD-19 dataset**. It features an intelligent **Q&A agent** capable of answering biomedical research questions based on real scientific literature.

---

## 🚀 Project Highlights

- 🔍 **Filtered CORD-19 Dataset** for relevant papers using keywords like "smoking", "nicotine", "vapping" and "covid"
- 🤖 Built a **retrieval-augmented generation (RAG)** pipeline with:
  - **LlamaIndex** for document indexing and query routing
  - **HuggingFace Embeddings** (`all-MiniLM-L6-v2`)
  - **FAISS** vector store for fast similarity search
- 🧬 Integrated **BioBERT** for biomedical context enhancement
- 🧠 Deployed a custom **LLM agent** to semantically answer questions like:
  > _"What is the effect of smoking on COVID-19 symptoms?"_
- 📊 Performed data cleaning, summarization, and chunking of scientific papers
- 📊 Performed **Sentiment Analysis** on scientific abstracts using a pre-trained model to categorize literature as *positive*, *neutral*, or *negative* toward smoking
- 🌐 Deployed a user-friendly **Gradio web interface** for question answering and result visualization

---

## 🛠️ Tech Stack

| Component       | Tool/Library                     |
|----------------|----------------------------------|
| Data Source     | [CORD-19 Dataset]|
| Embeddings      | HuggingFace `all-MiniLM-L6-v2`   |
| Vector Store    | FAISS                            |
| Language Models | LlamaIndex + optional BioBERT    |
| Agent Framework | LlamaIndex Query Engine          |
| Platform        | Google Colab                     |
| Language        | Python                           |

---

## 📂 Project Structure

```bash
📁 covid-smoking-agent/
│
├── data/                # Filtered and cleaned CORD-19 data
├── notebooks/           # Development notebooks in Google Colab
├── src/                 # Core scripts for loading, chunking, embedding, querying
│   ├── filter_cord19.py
│   ├── build_index.py
│   ├── query_agent.py
│
├── README.md            # Project overview
├── requirements.txt     # Dependencies
└── .gitignore
