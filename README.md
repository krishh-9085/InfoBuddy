# InfoBuddy: The College Query Chatbot

InfoBuddy is a sophisticated, user-friendly chatbot designed to answer college-related queries with speed and accuracy. Built with Streamlit, it features a Retrieval-Augmented Generation (RAG) pipeline to provide factual and context-aware responses.



## ✨ Features

*   **Interactive Chat Interface:** A clean and modern UI built with Streamlit.
*   **RAG Pipeline:** Ensures accurate and relevant answers by retrieving information from a local ChromaDB vector store.
*   **High-Performance LLM:** Powered by the Groq API, using the `llama-3.3-70b-versatile` model for fast and intelligent responses.
*   **Voice Input:** Allows for hands-free interaction using speech-to-text.
*   **Custom UI:** A polished and visually appealing chat interface with custom CSS, including typing animations and user/assistant icons.

## 🛠️ Technologies Used

*   **Frontend:** Streamlit
*   **Core Framework:** LangChain
*   **LLM Provider:** Groq, OpenAI
*   **Vector Store:** ChromaDB
*   **Embeddings:** HuggingFace Sentence Transformers (`all-mpnet-base-v2`)
*   **Speech Recognition:** `speechrecognition` library
*   **Environment Variables:** `python-dotenv`

## ⚙️ Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/InfoBuddy.git
    cd InfoBuddy
    ```

2.  **Create a virtual environment and activate it:**
    ```bash
    # For Windows
    python -m venv .venv
    .venv\Scripts\activate

    # For macOS/Linux
    python3 -m venv .venv
    source .venv/bin/activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a file named `.env` in the root of your project directory and add the following keys. You can get these from their respective platforms.

    ```
    GROQ_API_KEY="your-groq-api-key"
    OPENAI_API_KEY="your-openai-api-key"
    LANGCHAIN_API_KEY="your-langchain-api-key"
    ```

## 🚀 How to Run

1.  **Populate the Vector Database:**
    Before running the application, you need to populate the ChromaDB vector store located in the `datastore_db_new` directory. If you have a script for this (e.g., `populate_db.py`), run it first.
    
    *(Note: You should provide instructions here on how to run the script that populates the database with your college-specific data.)*

2.  **Run the Streamlit application:**
    Once your environment is set up and the database is populated, you can start the application with the following command:
    ```bash
    streamlit run InfoBuddy.py
    ```
    The application will be accessible in your web browser at `http://localhost:8501`.

## 📁 Project Structure

```
.
├── .env                  # Environment variables
├── datastore_db_new/     # ChromaDB vector store
├── InfoBuddy.py          # Main Streamlit application
├── requirements.txt      # Project dependencies
└── styles.css            # Custom CSS for the UI
```
