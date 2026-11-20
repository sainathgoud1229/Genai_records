# Generative AI Laboratory Experiments

A practical collection of **10 Generative AI experiments** implemented in Jupyter Notebooks. This repository documents hands-on work with core GenAI concepts, language-model workflows, embeddings, Retrieval-Augmented Generation (RAG), automated exploratory data analysis, API deployment, and basic misinformation/phishing detection.

The notebooks are organized in experiment order and include code, execution steps, and outputs where applicable.

<p align="center">
  <img src="https://img.shields.io/badge/Experiments-10-blue?style=for-the-badge" alt="10 experiments" />
  <img src="https://img.shields.io/badge/Python-3.x-yellow?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter Notebook" />
  <img src="https://img.shields.io/badge/Focus-Generative%20AI-purple?style=for-the-badge" alt="Generative AI" />
</p>

## Table of Contents

- [About the Repository](#about-the-repository)
- [Objectives](#objectives)
- [Experiment Index](#experiment-index)
- [Technology Stack](#technology-stack)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [API Key Configuration](#api-key-configuration)
- [Running the FastAPI Experiment](#running-the-fastapi-experiment)
- [Important Notes](#important-notes)
- [Learning Outcomes](#learning-outcomes)
- [Future Improvements](#future-improvements)
- [Author](#author)

## About the Repository

This repository contains the practical notebooks completed as part of a Generative AI laboratory record. The work moves from foundational concepts toward applied workflows and deployment.

Topics represented in the notebooks include:

- Content generation and language-model interaction
- Tokenization and GPT-related concepts
- The notebook topic identified as CSA3
- Text embeddings and semantic representation
- Retrieval-Augmented Generation (RAG)
- The notebook topics identified as CMS and CLNLM
- Automated Exploratory Data Analysis (Auto EDA) with AI-generated insights
- Exposing an LLM workflow through a FastAPI application
- Rule-based detection of potential misinformation and phishing messages

**Note:** The experiment filenames are retained as they appear in the repository so that each entry can be opened directly without changing the lab-record naming.

## Objectives

1. Understand the basic workflow and applications of Generative AI.
2. Explore how text is processed and represented for language-model applications.
3. Work with embeddings and retrieval-based question answering concepts.
4. Practice connecting language models with application code.
5. Generate and interpret automated data-analysis insights.
6. Build and test a simple API endpoint that invokes a language model.
7. Implement a basic text classifier that flags selected phishing and misinformation indicators.
8. Maintain reproducible, organized practical work using Jupyter Notebook and GitHub.

## Experiment Index

| No. | Experiment / Topic | Notebook |
|---:|---|---|
| 01 | Content Generation – Experiment 1 | [1.content_Experiment_1.ipynb](./1.content_Experiment_1.ipynb) |
| 02 | Tokenization – GPT | [2.Tokenization_2.GPT.ipynb](./2.Tokenization_2.GPT.ipynb) |
| 03 | CSA3 | [3.CSA3.ipynb](./3.CSA3.ipynb) |
| 04 | Text Embeddings | [4.Embeddings.ipynb](./4.Embeddings.ipynb) |
| 05 | Retrieval-Augmented Generation (RAG) | [5.RAG.ipynb](./5.RAG.ipynb) |
| 06 | CMS | [6.CMS.ipynb](./6.CMS.ipynb) |
| 07 | CLNLM | [7.CLNLM.ipynb](./7.CLNLM.ipynb) |
| 08 | Automated Exploratory Data Analysis (Auto EDA) | [8.Auto_EDA.ipynb](./8.Auto_EDA.ipynb) |
| 09 | LLM Application Deployment using FastAPI | [9.Deploy_LLM_FASTAPI.ipynb](./9.Deploy_LLM_FASTAPI.ipynb) |
| 10 | Misinformation and Phishing Detection | [10.Misinfromation.ipynb](./10.Misinfromation.ipynb) |

### Highlights from selected experiments

#### Experiment 4 – Text Embeddings
Explores the conversion of text into numerical vector representations. Embeddings are useful for representing semantic meaning and are commonly used in similarity search and retrieval-based applications.

#### Experiment 5 – Retrieval-Augmented Generation (RAG)
Covers the RAG workflow, where relevant information is retrieved and supplied as context to a language model to help it answer questions grounded in the retrieved material.

#### Experiment 8 – Automated EDA
Uses Python-based data analysis and an LLM-assisted workflow to inspect a dataset and produce readable insights. The notebook includes analysis of dataset characteristics such as missing values and AI-generated observations.

#### Experiment 9 – LLM Deployment with FastAPI
Creates a FastAPI application with a `/generate` endpoint. The endpoint accepts a question, invokes a Gemini language model through LangChain, and returns the generated answer with basic response checks. A Swagger UI is available for interactive API testing.

#### Experiment 10 – Misinformation and Phishing Detection
Implements a simple rule-based text classifier. It checks messages for configured phishing phrases, misinformation-related phrases, and URL patterns, then assigns a warning label. This is a demonstration of keyword-based detection, not a fact-checking system.

## Technology Stack

The notebooks use Python and the relevant libraries required by each experiment. The following tools and technologies are represented in the repository:

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Jupyter Notebook | Interactive development and experiment documentation |
| Google Gemini API | Language-model access in the Gemini-based workflows |
| LangChain | Integration with language-model workflows |
| Sentence Transformers | Text embedding generation in the embedding workflow |
| FastAPI | Building the LLM API application |
| Uvicorn | Running the FastAPI application |
| Pydantic | Defining and validating API request data |
| Requests | Sending HTTP requests to test the API |
| pandas / data-analysis libraries | Dataset inspection and exploratory analysis |
| re (Python regular expressions) | URL-pattern checks in the message-classification experiment |

Not every dependency is required for every notebook. Install the packages needed by the notebook you intend to run.

## Repository Structure

```text
Genai_records/
│
├── .gitignore
├── 1.content_Experiment_1.ipynb
├── 2.Tokenization_2.GPT.ipynb
├── 3.CSA3.ipynb
├── 4.Embeddings.ipynb
├── 5.RAG.ipynb
├── 6.CMS.ipynb
├── 7.CLNLM.ipynb
├── 8.Auto_EDA.ipynb
├── 9.Deploy_LLM_FASTAPI.ipynb
├── 10.Misinfromation.ipynb
└── README.md
```

Each `.ipynb` file is a self-contained notebook for its corresponding experiment.

## Getting Started

### 1. Clone the repository

Open a terminal and run:

```bash
git clone https://github.com/sainathgoud1229/Genai_records.git
cd Genai_records
```

### 2. Create a virtual environment (recommended)

**Windows PowerShell:**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Jupyter Notebook

```bash
python -m pip install --upgrade pip
pip install notebook ipykernel
```

### 4. Open the notebooks

```bash
jupyter notebook
```

Your browser will open the Jupyter interface. Select an experiment notebook and execute its cells from top to bottom.

> **Tip:** Some notebooks download pretrained models or call external APIs. Their first execution may take longer and may require an internet connection.

## API Key Configuration

Some language-model experiments require an API key. The Gemini-based notebooks use a Google Gemini API key.

1. Create or access a key through [Google AI Studio](https://aistudio.google.com/app/apikey).
2. When the notebook prompts for the key, enter it without displaying or hardcoding it in a notebook cell.
3. Keep API keys private. Never commit API keys, service-account JSON files, passwords, or other credentials to GitHub.

A safer Python pattern is:

```python
import os
import getpass

os.environ["GOOGLE_API_KEY"] = getpass.getpass("Enter your Gemini API key: ")
```

If a key was accidentally committed or exposed, revoke or rotate it with the provider. Removing it from the latest notebook version does not make an already exposed key safe.

## Running the FastAPI Experiment

Experiment 9 demonstrates a simple LLM-powered API.

After installing the dependencies and configuring the Gemini API key, run the notebook cells in order. The notebook starts the FastAPI application locally.

- Base URL: `http://127.0.0.1:8000`
- Interactive API documentation: `http://127.0.0.1:8000/docs`
- Generation endpoint: `POST /generate`

Example request body:

```json
{
  "question": "Explain generative artificial intelligence in simple terms."
}
```

The endpoint returns the submitted question, the model-generated answer, and basic evaluation information such as whether the answer is non-empty and its character count.

These checks confirm that a response was returned; they do **not** measure factual correctness, relevance, safety, or overall answer quality.

## Important Notes

- Run notebook cells in sequence unless the notebook explicitly says otherwise.
- Install missing packages in the active Python environment or Jupyter kernel.
- Model downloads and API calls may require internet access.
- API availability, model names, quotas, and provider policies can change.
- Never upload private datasets, credentials, or personal information.
- The misinformation/phishing notebook uses a small set of manually configured indicators. A message labelled as having no listed warning indicators is **not guaranteed to be safe**.
- A URL is not automatically malicious. The URL warning in Experiment 10 only recommends reviewing the link.
- The repository is an educational laboratory collection, not a production-ready security or fact-checking product.

## Learning Outcomes

After working through these experiments, the learner gains practical exposure to:

- The foundations and application patterns of Generative AI.
- Text tokenization and language-model workflows.
- Semantic vector representations using embeddings.
- Retrieval-based context grounding with RAG.
- Connecting model workflows to Python applications.
- Automated dataset exploration and AI-assisted insight generation.
- Creating and testing REST API endpoints using FastAPI.
- Basic rule-based text classification and its limitations.
- Notebook organization, environment setup, and version control with Git and GitHub.

## Future Improvements

Potential improvements to this practical collection include:

- Add a single documented environment file with verified, compatible package versions.
- Add screenshots of important notebook outputs.
- Add automated tests for reusable Python functions and API endpoints.
- Extend the FastAPI example with input validation, structured error handling, logging, and configuration management.
- Evaluate LLM responses using appropriate quality metrics and test datasets.
- Improve phishing and misinformation detection using labeled datasets and trained models, with human review for uncertain cases.
- Add deployment instructions for hosting the API.

## Author

**Kadirisani Sainath Goud**

- GitHub: [@sainathgoud1229](https://github.com/sainathgoud1229)
- Repository: [Genai_records](https://github.com/sainathgoud1229/Genai_records)

---

If you find this repository useful for learning Generative AI concepts, feel free to explore the notebooks in sequence.

