# Generative-AI-Document-Assistant-with-AWS-Bedrock

## Project Overview

This application enables users to interactively query PDF documents using advanced AI models. Leveraging **AWS Bedrock**, **LangChain**, and **Streamlit**, the solution provides real-time, context-aware answers from PDF files. It utilizes **Titan Embeddings** for document vectorization and integrates **Claude** and **Llama2** LLMs for retrieval-based question answering.

---

## Key Features

- **PDF Ingestion:** Automatically loads and processes PDF files from the `data` directory.
- **Text Chunking:** Splits documents into manageable chunks for efficient embedding and retrieval.
- **Vector Store:** Uses **FAISS** for fast similarity search and persistent vector storage.
- **Embeddings:** Employs **Amazon Titan Embeddings** via AWS Bedrock for high-quality vector representations.
- **LLM Integration:** Supports both **Claude** and **Llama2** models for generating detailed, context-rich answers.
- **Interactive UI:** Built with **Streamlit** for a user-friendly chat interface.
- **Scalable & Cloud-Native:** Designed for enterprise document intelligence workflows.

---

## How It Works

1. **Data Ingestion:** Loads PDFs and splits them into text chunks.
2. **Vectorization:** Generates embeddings for each chunk and stores them in a FAISS index.
3. **Question Answering:** Retrieves relevant chunks and uses selected LLMs to answer user queries.
4. **User Interaction:** Users can update the vector store and query documents via the Streamlit interface.

---

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/aws-bedrock-pdf-qa.git
   cd aws-bedrock-pdf-qa
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure AWS Credentials**
   - Ensure your AWS credentials are set up for Bedrock access.

4. **Add PDF Files**
   - Place your PDF documents in the `data` directory.

5. **Run the Application**
   ```bash
   streamlit run app.py
   ```

---

## Usage

- Use the sidebar to update or create the vector store from your PDFs.
- Enter your question in the main input box.
- Choose either **Claude Output** or **Llama2 Output** to get answers.

---

## Technologies Used

- **AWS Bedrock**
- **LangChain**
- **Streamlit**
- **FAISS**
- **Amazon Titan Embeddings**
- **Claude & Llama2 LLMs**

---

## License

This project is licensed under the MIT License.

---

## Contact

For questions or support, please open an issue or contact
