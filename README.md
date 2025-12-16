# Simple RAG System 🤖

A Retrieval-Augmented Generation (RAG) system that allows you to query PDF and TXT documents using semantic search and LLM-powered responses.

## Features

- 📄 Supports PDF and TXT documents
- 🔍 Semantic search using sentence embeddings
- 💬 Context-aware responses using Groq's LLaMA models
- 🚀 Lightweight and easy to use

## Setup

1. Get a Groq API key from [console.groq.com](https://console.groq.com)

2. Set your API key as an environment variable:

**Linux/Mac:**
```bash
export GROQ_API_KEY="your_api_key_here"
```

**Windows (Command Prompt):**
```cmd
set GROQ_API_KEY=your_api_key_here
```

**Windows (PowerShell):**
```powershell
$env:GROQ_API_KEY="your_api_key_here"
```

## Usage

1. Prepare a folder with your PDF and/or TXT documents

2. Run the system:
```bash
python rag_system.py
```

3. Enter the path to your documents folder when prompted

4. Start asking questions!

## Configuration

You can adjust these parameters in the code:

- `CHUNK_SIZE`: Number of characters per text chunk (default: 500)
- `CHUNK_OVERLAP`: Overlap between chunks (default: 50)
- `TOP_K_RESULTS`: Number of relevant passages to retrieve (default: 3)

## Requirements

- Python 3.7+
- groq
- sentence-transformers
- scikit-learn
- PyPDF2
- numpy

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.
