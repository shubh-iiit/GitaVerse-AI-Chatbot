<img src="flute.png" alt="GitaVerse Screenshot" width="200"/>

# GitaVerse: Intelligent Bhagavad Gita Chatbot

 GitaVerse is a state-of-the-art AI-powered chatbot designed specifically for deep, context-aware Q&A on the Bhagavad Gita. Leveraging advanced Retrieval-Augmented Generation (RAG), scalable vector search with ChromaDB Cloud, and the blazing-fast Groq LLM, this project demonstrates expertise in modern NLP, cloud infrastructure, and full-stack development. The solution is engineered for reliability, scalability, and an intuitive user experience—making it a valuable resource for students, scholars, and spiritual seekers alike.

---

## Why GITA-GPT?

Traditional search tools and static Q&A bots often fail to capture the nuanced wisdom of the Bhagavad Gita. GITA-GPT bridges this gap by combining:

- **Semantic Understanding:** Uses vector embeddings to understand the true meaning behind user queries, not just keywords.
- **Contextual Retrieval:** Surfaces the most relevant verses and explanations, even for complex or open-ended questions.
- **Modern AI Stack:** Integrates FastAPI for robust backend APIs, ChromaDB Cloud for scalable vector search, and Groq LLM for lightning-fast, high-quality language generation.
- **Custom Frontend:** Offers a seamless, interactive experience with a modern HTML/CSS/JS interface.

---

## Features

- **Ask any question** about the Bhagavad Gita and receive contextually accurate, AI-generated answers.
- **Semantic search** over all verses using advanced vector embeddings for deep understanding.
- **Retrieval-Augmented Generation (RAG):** Combines the power of search and generation for precise, referenced answers.
- **FastAPI backend** with Groq LLM integration for scalable, production-grade APIs.
- **ChromaDB Cloud** for managed, high-performance vector search—no local database setup required.
- **Modern frontend** (HTML/CSS/JS) with smooth UX, responsive design, and instant feedback.
- **Easy extensibility:** Modular codebase allows for quick adaptation to other texts or languages.
- **Secure and configurable:** API key management and environment-based configuration for safe deployment.

---

## Project Structure

```
.
├── api.py                  # FastAPI backend server
├── create_chroma_index.py  # Script to create ChromaDB index from Gita data
├── gita_data.json          # Bhagavad Gita data in JSON format
├── gita.csv                # Bhagavad Gita data in CSV format
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
├── .gitignore
└── static/
    ├── index.html          # Main frontend HTML
    ├── script.js           # Frontend JavaScript
    └── styles.css          # Frontend CSS
```

---

## User Guide

### Prerequisites

- Python 3.8+
- A [GROQ API key](https://console.groq.com/keys)
- Internet connection (for ChromaDB Cloud and frontend assets)

### Setup

1. **Clone the repository**
    ```sh
    git clone https://github.com/yourusername/GITA-GPT.git
    cd GITA-GPT-main
    ```

2. **Install dependencies**
    ```sh
    pip install -r requirements.txt
    ```

3. **Set your GROQ API key**
    - Export your key as an environment variable:
      ```sh
      export GROQ_API_KEY=your_groq_api_key
      ```
    - Or set it in your shell/profile.

4. **(Optional) Rebuild ChromaDB index**
    - If you modify `gita_data.json`, run:
      ```sh
      python create_chroma_index.py
      ```

5. **Start the API server**
    ```sh
    python api.py
    ```

6. **Access the frontend**
    - Open [http://localhost:8000/static/index.html](http://localhost:8000/static/index.html) in your browser.

---

## Usage

- Enter your question about the Bhagavad Gita in the input box.
- Adjust the number of verses to retrieve (slider).
- Click **Ask** to receive AI-powered answers and relevant verses.
- Explore related questions and copy responses as needed.

---

## Technical Highlights

- **RAG Pipeline:** Combines semantic search (ChromaDB) with generative AI (Groq LLM) for accurate, referenced answers.
- **Cloud-Native:** Uses ChromaDB Cloud for effortless scaling and reliability.
- **API-First:** FastAPI enables easy integration with other apps or platforms.
- **Frontend-Backend Decoupling:** Clean separation for maintainability and future expansion.
- **Production-Ready:** Secure API key handling, modular code, and clear documentation.

---

## License

MIT License

---

## Acknowledgements

- [FastAPI](https://fastapi.tiangolo.com/)
- [ChromaDB](https://www.trychroma.com/)
- [Groq LLM](https://groq.com/)
