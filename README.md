# Book Recommender Engine using LLMs

### Overview

This project is a Book Recommender Engine powered by Large Language Models (LLMs) and open-source models from Hugging Face. The system provides book recommendations based on vector embeddings, zero-shot classification, and sentiment analysis of book descriptions. The user interface is built using Gradio.

### Features

* Vector Indexing & Embeddings: Uses _intfloat/multilingual-e5-small_ to generate book embeddings for similarity-based recommendations.
* Zero-Shot Classification: Utilizes _facebook/bart-large-mnli_ to classify books into relevant categories.
* Sentiment Analysis: Analyzes book descriptions using _j-hartmann/emotion-english-distilroberta-base_.
* Interactive UI: Built with Gradio for easy user interaction.

### Tech Stack

* Python
* LangChain (for LLM orchestration)
* Transformers (Hugging Face models)
* Gradio (UI framework)
* ChromaDB (for vector storage and retrieval)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/book-recommender.git
cd book-recommender

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\activate  # On Windows
source .venv/bin/activate  # On macOS/Linux

# Install dependencies
pip install kagglehub pandas matplotlib seaborn python-dotenv langchain-community langchain-chroma langchain-openai transformers sentence-transformers gradio ipywidgets

```
### Running the Application

```bash
python app.py
```

### Usage
1. Enter a book description in the input box.
2. Select a category that best matches the type of book you're looking for.
3. Choose an emotional tone that fits your preference.
4. Click "Find Recommendations" to get a list of classified book recommendations.
5. Browse the recommended books and choose your next read!


