# Article Research Tool 📈

The **Article Research Tool** is a web application that allows users to upload links to online articles and ask questions. The tool uses Generative AI and LangChain to process the articles, extract relevant information, and provide accurate responses along with the sources.

---

## Features

- **Upload Article Links**: Add up to three article URLs for processing.
- **AI-Powered Q&A**: Ask questions related to the articles, and get concise answers.
- **Source Citation**: Responses include references to the original article sources.

---

## Technology Stack

- **Framework**: [Streamlit](https://streamlit.io/) for creating the interactive UI.
- **LLM Integration**: OpenAI's API for natural language processing.
- **Document Processing**:
  - **LangChain** for chaining operations.
  - **FAISS** for efficient vector storage and retrieval.
- **Environment Management**: dotenv for securely handling API keys.
- **Pickle** for saving and loading embeddings.

---

## Prerequisites

1. Python 3.7+
2. Vlaid OpenAI API Key
3. Libraries:
   - Streamlit
   - LangChain
   - OpenAI
   - FAISS
   - Unstructured
   - Python-dotenv

Install the dependencies using:
```bash
pip install -r requirements.txt
