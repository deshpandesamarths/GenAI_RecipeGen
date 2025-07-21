# RecipeGen: AI-Powered Semantic Recipe Recommendation and Generation

## Project Overview

RecipeGen is an AI-driven application designed to assist users in discovering and generating cooking recipes based on the ingredients they have, specific dietary preferences, or custom free-form prompts. The system combines semantic understanding through Sentence-BERT, efficient similarity search using FAISS, and recipe generation using the Phi-2 language model from Hugging Face.

This project demonstrates how modern natural language processing techniques can be applied to real-world tasks such as recipe recommendation and generation, delivering an intuitive and personalized cooking assistant.

---

## Features

### Ingredient-Based Recipe Recommendation

Users can enter a list of ingredients they have, and the application will return the most relevant recipe from a curated dataset using semantic similarity.

### AI-Based Recipe Generation

By entering a natural language prompt (e.g., “Create a vegan breakfast with oats and banana”), users receive a freshly generated recipe written by an AI model.

### Semantic Matching Using Sentence-BERT and FAISS

All recipe texts and user inputs are converted into sentence embeddings using Sentence-BERT. These embeddings are indexed using FAISS, enabling fast and accurate retrieval of the most relevant recipes.

### Simple and Interactive Web Interface

A web-based user interface built with Gradio allows users to interact with the application easily—no technical knowledge required.

---

## Tech Stack

| Component            | Purpose                                     |
| -------------------- | ------------------------------------------- |
| Sentence-BERT        | Embedding user inputs and recipe texts      |
| FAISS                | Fast vector similarity search               |
| Phi-2 (Hugging Face) | Generative language model for recipes       |
| Gradio               | Interface for user interaction              |
| Additional Tools     | Transformers, Torch, Datasets, Scikit-learn |

---

## Installation and Running the Application

### Prerequisites

Ensure Python (version 3.8 or above) is installed. Then, install the required Python libraries using:

```bash
pip install gradio sentence-transformers faiss-cpu transformers torch
```

### Running the App

To start the application locally, run:

```bash
python app.py
```

Once launched, the app will be available in your browser at `http://127.0.0.1:7860`.

---

## Project Structure

```
GenAI_RecipeGen/
├── app.py                  # Main Gradio app script
├── recipegen_utils.py      # Functions for search and generation
├── recipes.json            # Curated recipe dataset
├── embeddings.faiss        # FAISS index (optional or auto-generated)
├── RecipeGen.ipynb         # Jupyter notebook for experimentation
├── requirements.txt        # List of Python dependencies
├── LICENSE                 # License file (MIT)
└── README.md               # Project documentation
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

---

## Acknowledgments

This project was made possible thanks to the open-source tools and models provided by:

* Hugging Face (Transformers and Phi-2)
* SentenceTransformers community
* Facebook AI Research (FAISS)
* Gradio for the UI framework
* The broader Python and machine learning community

---

Let me know if you'd like me to:

* Save this as a `.md` file for direct use in your repo.
* Help set up a `LICENSE` file.
* Add GitHub badges or CI/CD actions to polish the repository.
