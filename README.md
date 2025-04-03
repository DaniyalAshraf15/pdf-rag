# AI-Powered PDF Processing & Semantic Search

This project provides a web-based solution for uploading PDF documents, generating vector embeddings, and performing semantic search using OpenAI’s language models. It efficiently extracts text from PDFs, converts them into vector embeddings, stores them in Pinecone, and enables users to retrieve relevant information using natural language queries.

## Features

- **PDF Upload & Processing**: Users can upload PDFs through a web interface.
- **Text Extraction & Chunking**: Extracts text and splits it into smaller chunks using LangChain for better context retention.
- **Vector Embeddings Generation**: Utilizes OpenAI's `text-embedding-ada-002` model to create embeddings.
- **Efficient Storage**: Stores embeddings in Pinecone for fast and scalable retrieval.
- **Semantic Search & Query Handling**: Queries are transformed into embeddings and matched against stored vectors to fetch the most relevant context.
- **AI-Powered Response Generation**: OpenAI's language models generate refined answers based on retrieved content.

## Installation & Setup

### Prerequisites
Ensure you have Python installed (preferably Python 3.8+). Install dependencies using:
```sh
pip install -r requirements.txt
```

### Environment Variables
Set up API keys and host details:
```sh
export OPENAI_API_KEY='your-openai-api-key'
export PINECONE_API_KEY='your-pinecone-api-key'
export PINECONE_HOST='your-pinecone-host'
```

## Usage

1. **Start the application**
   ```sh
   python app.py
   ```
2. **Access the application**
   - **Local:** `http://127.0.0.1:5000/`
   - **Remote:** `http://your-vm-ip:5000/` (Ensure port 5000 is open in the firewall)
3. **Upload a PDF** through the web interface.
4. **Process the file** to generate embeddings.
5. **Enter a query** and select an OpenAI model.
6. **Retrieve relevant search results** and AI-generated responses.
7. **End the session** to clean up stored data.

## Contributing
Feel free to fork this repository and submit pull requests for improvements. Ensure to follow proper code structure and documentation practices.

## License
This project is licensed under the MIT License. See `LICENSE` for details.

---

This application allows efficient document search and retrieval, making it ideal for AI-powered knowledge management and research purposes.

