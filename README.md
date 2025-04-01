# CHAT_WITH_MULTIPLE_DOCS
Chat with PDF,DOCX, TXT, PPTX, CSV, and Excel (XLSX, XLS) files using GEMINI..
# Chat with Documents

## Overview
This **Chat with Documents** application is a Streamlit-based tool that allows users to upload PDF, DOCX, TXT, PPTX, CSV, and Excel (XLSX, XLS) files, process their content, and ask questions about them using Google's Gemini AI model. The tool leverages LangChain, FAISS for vector storage, and Google Generative AI for efficient question-answering.

## Features
- Extracts text from PDF, DOCX, TXT, PPTX, CSV, and Excel files.
- Splits extracted text into manageable chunks.
- Generates embeddings using Google Generative AI embeddings.
- Stores and retrieves embeddings efficiently using FAISS.
- Answers user queries using Gemini AI via LangChain’s conversational chain.
- Provides accurate responses based on the uploaded documents.

## Tech Stack
- **Python** (Core programming language)
- **Streamlit** (User interface)
- **LangChain** (For LLM-based workflows)
- **Google Gemini AI** (LLM for text generation)
- **FAISS** (Vector database for retrieval)
- **PyPDF2** (For extracting text from PDFs)
- **python-docx** (For handling DOCX files)
- **python-pptx** (For handling PPTX files)
- **pandas** (For handling CSV and Excel files)

## Installation
### Prerequisites
Ensure you have Python installed (>=3.8) and `pip` package manager.

### Steps
  
1. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
   If you encounter issues with PPTX files, install `python-pptx` manually:
   ```sh
   pip install python-pptx
   ```
2. Set up your API key for Google Gemini AI:
   - Open `app.py` and replace `GOOGLE_API_KEY` with your actual API key.
3. Run the application:
   ```sh
   streamlit run app.py
   ```

## Usage
1. Upload PDF, DOCX, TXT, PPTX, CSV, or Excel files using the sidebar.
2. Click **Submit & Process** to extract and process document content.
3. Ask questions in the input field to retrieve an answer.
4. View the AI-generated response based on your documents.

## File Structure
```
chat-with-docs/
│── app.py               # Main Streamlit application
│── requirements.txt     # Dependencies
│── faiss_index/         # FAISS vectorstore (saved locally)
│── README.md            # Documentation
```

## License
This project is open-source and available under the [MIT License](LICENSE).

---
**Developed by:** [JAGADEESH KATTA]


