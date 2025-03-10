# Gemma Model Document Q&A

## Overview
This project is a **Document Q&A System** that utilizes **Google Gemma** for answering questions based on ingested PDF documents. It leverages **LangChain**, **FAISS**, and **Google Generative AI Embeddings** for document retrieval and contextual understanding. The system enables users to query information from embedded documents with high accuracy.

## Features
- **PDF Document Ingestion**: Loads and processes PDF documents from a specified directory.
- **Text Chunking**: Splits documents into manageable chunks for efficient retrieval.
- **Vector Storage with FAISS**: Stores embeddings for fast similarity search.
- **Question Answering**: Uses **ChatGroq** with **Llama3-8b-8192** to generate responses based on retrieved context.
- **Streamlit UI**: Provides an interactive interface for users to embed documents and ask questions.

## Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- pip
- Virtual environment (optional but recommended)

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Configuration
1. Set up API keys in a `.env` file:
   ```env
   GROQ_API_KEY=your_groq_api_key
   GOOGLE_API_KEY=your_google_api_key
   ```
2. Ensure that the required PDF files are placed in the **us_census** directory.

## Usage
1. Run the Streamlit application:
   ```bash
   streamlit run app.py
   ```
2. Open the application in your browser.
3. Click **"Documents Embedding"** to process and store document embeddings.
4. Enter a question in the text input field and retrieve answers from the documents.

## Dependencies
The following Python libraries are used:
- `streamlit`
- `langchain`
- `langchain_groq`
- `langchain_google_genai`
- `faiss-cpu`
- `python-dotenv`
- `PyPDF2`

To install all dependencies, use:
```bash
pip install -r requirements.txt
```

## Notes
- Ensure the `.env` file is properly configured with valid API keys.
- The PDF directory path should be updated if necessary.
- Response time may vary based on document size and query complexity.

## License
This project is licensed under the **MIT License**.

## Contact
For queries, reach out to [sisiras325@gmil.com].

 
