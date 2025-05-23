 "Automated Technical Documentation Generation using LLM":




> Final Year Graduation Project | Nile University - School of IT & Computer Science | Spring 2024

Project Overview

This project demonstrates the development of an automated code documentation system powered by large language models (LLMs) such as Code Llama. It aims to simplify the software development process by generating high-quality, human-readable documentation and diagrams from source code and GitHub repositories.

Key Features

* 📄 Generate Documentation: Automatically create descriptive documentation for functions, classes, and scripts in multiple programming languages.
* 🔍 GitHub Repository Analysis: Clone and analyze public repositories to produce documentation and allow natural language queries.
* 🧾 Code Annotation: Add inline comments to improve code readability and maintainability.
* 🖼️ Diagram Generation: Visualize class structures using Mermaid.js.
* 🌍 Multi-language Support: Compatible with Python, Java, C++, JavaScript, SQL, HTML, CSS, PHP, Ruby, and Swift.
* 🧠 LLM-Powered**: Utilizes the CodeLlama-7B-Instruct-HF model from HuggingFace for documentation generation.

Authors

* Ahmed Eltohamy
* Ahmed Sarg
* Yusuf Farouk
* Youssef Haitham
* Youssef Abozeid
* Youssef Poules

**Supervised by**:
Dr. Tamer Arafa & Eng. Mina Atef

## 🏗️ Tech Stack

| Technology                | Use                                  |
| ------------------------- | ------------------------------------ |
| Python                    | Core programming language            |
| Streamlit                 | Web application framework            |
| Hugging Face Transformers | LLM integration (Code Llama)         |
| Torch                     | Deep learning computations           |
| LangChain                 | Document analysis & querying         |
| GitPython                 | GitHub integration                   |
| Chroma                    | Vector store for document embeddings |
| Mermaid.js                | Diagram rendering                    |

Project Structure

```
📦 auto-docs
├── app.py                  # Main Streamlit app
├── utils/                  # Code extraction & parsing
├── github/                 # GitHub repository analysis
├── diagrams/               # Mermaid generation logic
├── models/                 # LLM loading and inference
└── README.md               # You are here!
```

How to Run

1. **Install Dependencies**

```bash
pip install -r requirements.txt
```

2. **Launch the App**

```bash
streamlit run app.py
```

3.Navigate through the UI

* Home: Paste code snippets.
* Document Files: Upload files for analysis.
* GitHub Query: Enter repository URL for full analysis and QA.

## 🧪 Evaluation

* ROUGE-1: 0.31
* ROUGE-L: 0.26
* BLEU: 0.095

> Despite low BLEU due to verbosity, human evaluation confirmed high-quality documentation and improved comprehension.

Limitations

* Constrained by GPU memory (used Google Colab T4).
* Incomplete support for all diagram types (e.g., sequence diagrams).
* BLEU metrics are less reflective due to descriptive nature of LLM outputs.

Future Work

* Integration with IDEs for real-time documentation.
* Advanced diagrams (sequence, use case, state).
* Use of larger models (e.g., CodeLlama-13B) for enhanced accuracy.


