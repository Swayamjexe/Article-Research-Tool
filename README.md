# Article Research Tool 📈

The **Article Research Tool** is an intuitive web application that leverages cutting-edge AI to help you research online articles. Simply provide article URLs, ask questions, and receive accurate answers along with citations from the original sources. Perfect for researchers, journalists, and curious minds!

---

## ✨ Features

- **Upload Article Links**: 
  - Input up to three article URLs via the sidebar for processing.
- **AI-Powered Q&A**: 
  - Ask natural language questions about the content of the articles.
  - Receive concise, well-structured answers powered by OpenAI.
- **Source Citation**: 
  - Answers include references to the specific sections of the articles they’re based on, ensuring transparency and trust.
- **Streamlined Workflow**: 
  - Real-time feedback on the status of data processing and embedding generation.

---

## 🛠️ Technology Stack

- **Framework**: 
  - [Streamlit](https://streamlit.io/) for building an interactive and user-friendly web interface.
- **Natural Language Processing**:
  - OpenAI's GPT API for robust language understanding and generation.
  - [LangChain](https://www.langchain.com/) for constructing reliable AI chains.
- **Document Handling**:
  - [Unstructured](https://github.com/Unstructured-IO/unstructured) for loading and processing article content.
  - Recursive character text splitting for efficient handling of large documents.
- **Embeddings and Vector Search**:
  - [FAISS](https://faiss.ai/) for creating and retrieving vector embeddings of processed data.
- **Environment Management**:
  - [python-dotenv](https://github.com/theskumar/python-dotenv) for secure handling of API keys and environment variables.
- **Data Serialization**:
  - Pickle for saving and loading FAISS indexes for seamless reuse.

---

## 📋 Prerequisites

Ensure the following tools and libraries are installed before running the application:

1. **Python Version**: Python 3.7 or higher.
2. **API Key**: A valid OpenAI API key.
3. **Required Libraries**: Install the dependencies listed below:
   ```bash
   pip install -r requirements.txt
   ```

   Dependencies include:
   - `streamlit`
   - `langchain`
   - `openai`
   - `faiss-cpu`
   - `unstructured`
   - `python-dotenv`

---

## 🚀 How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Swayamjexe/Article-Research-Tool.git
   cd article-research-tool
   ```

2. **Set Up the Environment**:
   - Create a `.env` file in the project directory and add your OpenAI API key:
     ```
     OPENAI_API_KEY=your_api_key_here
     ```

3. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

4. **Interact with the Tool**:
   - Use the sidebar to input up to three article URLs.
   - Click **Process URLs** to extract and process the content.
   - Ask your questions in the input box, and get insightful answers along with cited sources.

---

## 📂 Project Structure

```plaintext
📁 article-research-tool/
├── app.py              # Main application script
├── requirements.txt    # List of dependencies
├── .env.example        # Example .env file
├── README.md           # Project documentation
└── faiss_store_openai.pkl  # Saved FAISS vector store (created at runtime)
```

---

## 🌟 Future Enhancements

- Allow users to upload articles as files (PDFs, Word docs, etc.).
- Expand support for additional language models and APIs.
- Improve UI/UX with dynamic visualizations and expanded settings.

---

