# Chatbot for Interacting with PDFs

This Python script implements a chatbot using Streamlit, a web application framework for Python. The chatbot is designed to interact with PDF documents, allowing users to ask questions and receive answers based on the content of the PDFs.

## Features

- **PDF File Upload**: Users can upload PDF files through the Streamlit interface.
- **PDF Processing**: The uploaded PDF files are processed to extract text content using PyPDFLoader and RecursiveCharacterTextSplitter.
- **Question-Answering**: Users can ask questions related to the content of the PDF documents.
- **Language Model**: The chatbot uses the Ollama language model (LLM) for generating responses to user queries.
- **Vector Storage**: Vector representations of text chunks from the PDF documents are stored using Chroma.
- **Memory**: Conversation history is stored using ConversationBufferMemory to provide context-aware responses.

## Usage

1. **Upload PDF**: Start by uploading a PDF file using the file uploader widget.
2. **Ask Questions**: Once the PDF file is uploaded, you can ask questions related to the content of the document.
3. **Chat Interface**: The chat interface displays the conversation between the user and the chatbot. The chatbot's responses are generated based on the content of the PDF document.

## Dependencies

- Streamlit
- langchain

## Setup Instructions


1. Install the required dependencies using pip:

pip install streamlit langchain

2. Run the script using the following command:

streamlit run app.py

Replace `app.py` with the filename of your Python script containing the provided code.

## Notes

- Ensure that the necessary directories (`pdfFiles` and `vectorDB`) are created in the working directory to store PDF files and vector representations.
- The script requires the Ollama language model to be running locally at `http://localhost:11434`.

Feel free to customize the script and the README file according to your specific needs and preferences.



