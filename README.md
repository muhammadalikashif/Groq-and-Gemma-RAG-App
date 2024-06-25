# Gemma Model Document Q&A

This repository contains a Streamlit application that allows users to ask questions based on the context of provided documents. The application uses LangChain, Google Generative AI Embeddings, and FAISS for document retrieval and LLM-based question answering.

## Features

- Load and preprocess PDF documents.
- Create vector embeddings of document chunks.
- Retrieve relevant document chunks based on user queries.
- Generate accurate answers using the LangChain `ChatGroq` model.

## Installation

### Prerequisites

- Python 3.7+
- Virtual environment (recommended)

### Setup

1. **Clone the repository:**
    ```bash
    https://github.com/muhammadalikashif/Groq-and-Gemma-RAG-App.git
    
    ```

2. **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**

    Create a `.env` file in the root directory of the project and add your API keys:
    ```env
    GROQ_API_KEY=your_groq_api_key
    GOOGLE_API_KEY=your_google_api_key
    ```

5. **Add your PDF documents:**
   
    Place your PDF documents in the `./data` directory.

## Usage

1. **Run the Streamlit application:**
    ```bash
    streamlit run app.py
    ```

2. **Use the application:**
    - Open your browser and navigate to `http://localhost:8501`
    - Click on the "Documents Embedding" button to initialize the vector store.
    - Enter your question in the text input field and press Enter.
    - The application will retrieve the most relevant document chunks and generate an accurate answer.

## File Structure

- `app.py`: Main application script.
- `requirements.txt`: Python dependencies.
- `data/`: Directory to store PDF documents.
- `.env`: Environment variables file.

## Dependencies

- `streamlit`
- `langchain`
- `faiss`
- `langchain-groq`
- `langchain-google-genai`
- `python-dotenv`

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

