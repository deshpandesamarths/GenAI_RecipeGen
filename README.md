
# RecipeGen: AI-Powered Semantic Recipe Recommendation and Generation

## Project Overview

**RecipeGen** is an AI-based application that helps users discover and generate cooking recipes based on available ingredients, dietary preferences, or custom prompts. It combines semantic understanding using Sentence-BERT, fast similarity search with FAISS, and language generation via the Phi-2 model from Hugging Face.

The project highlights the power of combining retrieval-based methods and generative AI to create personalized recipe experiences.

---

## Features

### Ingredient-Based Recipe Recommendation

Input a list of ingredients to retrieve the most semantically relevant recipe from a curated dataset.

### Custom AI Recipe Generation

Use natural prompts like “Make a gluten-free breakfast with oats and berries,” and receive a freshly generated recipe using the Phi-2 language model.

### Semantic Search with Sentence-BERT and FAISS

User inputs and recipes are converted into embeddings with Sentence-BERT. FAISS is used for efficient nearest-neighbor retrieval.

### Gradio Interface (Jupyter-Notebook-Based)

The interface is built using Gradio and is launched directly from the Jupyter Notebook. No separate app file is needed.

---

## Tech Stack

| Tool/Library         | Purpose                                     |
| -------------------- | ------------------------------------------- |
| Sentence-BERT        | Generating embeddings for semantic matching |
| FAISS                | Fast nearest-neighbor search                |
| Phi-2 (Hugging Face) | Recipe generation using a language model    |
| Gradio               | Web-based interactive UI                    |
| Others:              | Transformers, Torch, Datasets, Scikit-learn |

---

## Installation and Setup

### Prerequisites

Ensure you have Python 3.8+ and Jupyter installed. Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## Running the App

Since the application runs via the Jupyter Notebook interface, follow these steps:

1. Launch Jupyter Notebook or Jupyter Lab in the project directory:

```bash
jupyter notebook
```

2. Open `RecipeGen.ipynb`.

3. Run all the cells in sequence.

4. Once the Gradio cell is executed, a local URL will appear (e.g., `http://127.0.0.1:7860/`). Open it in your browser to interact with the application.

---

## Project Structure

```
GenAI_RecipeGen/
├── RecipeGen.ipynb         # Main notebook with search + generation + Gradio UI
├── recipegen_utils.py      # Helper functions
├── recipes.json            # Recipe dataset
├── requirements.txt        # Python dependencies
├── LICENSE                 # MIT License
└── README.md               # Project documentation
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

---

## Acknowledgments

This project utilizes resources from:

* Hugging Face Transformers (including the Phi-2 model)
* SentenceTransformers
* Facebook AI Research (FAISS)
* Gradio
* The open-source Python ML ecosystem

---

Let me know if you'd like me to:

* Save this as a `README.md` file for your repo
* Add it to your Git project automatically
* Help you create a `requirements.txt` based on the actual notebook

Would you like me to do any of that now?
