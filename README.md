#  Conversational RAG with PDF Uploads and Chat History

This is a Streamlit application that allows you to **upload PDF documents** and **interact with their content** through a conversational chatbot. The chatbot uses a **Retrieval-Augmented Generation (RAG)** approach powered by the **Groq LLM (Gemma2-9B)** and maintains **chat history** for context-aware conversations.


##  Features

-  Upload one or multiple PDF files
-  Ask questions based on PDF content
-  Chatbot remembers past conversations (chat history)
-  Uses semantic search via vector embeddings (HuggingFace)
-  Powered by Groq's Gemma2-9B LLM
-  Clean and simple UI built with Streamlit


##  Tech Stack

- **LangChain** - for building RAG chains
- **Chroma** - vector store for document embeddings
- **HuggingFace Embeddings** - to embed PDF chunks
- **Groq LLM** - for answering user questions
- **Streamlit** - web app interface
- **PyPDFLoader** - for reading PDF content


## Setup Instructions

### 1. Clone the repository

```cmd 
git clone https://github.com/your-username/conversational-pdf-rag.git
cd conversational-pdf-rag
````

### 2. Create a `.env` file

```env
HF_TOKEN=your_huggingface_token
```

### 3. Install dependencies

```cmd
pip install -r requirements.txt
```

### 4. Run the app

```cmd
streamlit run app.py
```

## Usage

1. Enter your **Groq API Key**
2. Upload one or more **PDF files**
3. Enter a **Session ID** (optional, used to separate chat histories)
4. Ask your question in natural language
5. Chatbot will retrieve relevant content and respond