# 🧠 Automated Critique & Review System using LLMs

This project implements an end-to-end pipeline for automated academic paper critique using Large Language Models. Given a PDF research paper, the system performs:

- 📄 Parsing into sections and Paragraphs, extraction of figures and tabulation along with Section-wise summarization
- ✍️ Paragraph-level critique generation using a fine-tuned Mistral model
- ⚖️ Bias detection using sentiment analysis (VADER)
- 📋 Plagiarism detection using embedding similarity with PeerRead dataset

---

## 🔍 Features

- **PDF Parsing:** Extracts and splits papers into structured sections, figures, tables and paragraphs
- **Summarization:** Generates concise section summaries using BART
- **Critique Generation:** Calls a Hugging Face API to get peer-review style feedback
- **Bias & Plagiarism Flags:** Paragraphs are evaluated for potential bias and plagiarism
- **Data Source:** Evaluation uses real abstracts from the PeerRead dataset

---

## Model Info
- **Critique Generator:** Hugging Face model: Manoghn/mistral-qlora-critique
- **Summary Generator:** facebook/bart-large-cnn
- **Embedding Model (Plagiarism):** all-MiniLM-L6-v2
- **Bias using Sentiment Analyzer:** NLTK VADER

---

## 🚀 How to Run

### 1. Upload PDF
Run the notebook and upload any research paper in `.pdf` format.

### 2. Install Dependencies
Make sure to install all the required packages (see below or `requirements.txt`).
Make sure to use personal access token from the Hugging face library before running

### 3. Execute
The pipeline will print:
- Section-wise summaries
- Paragraph-wise critiques
- Bias and plagiarism analysis

---

## 🧰 Dependencies

Install using:

```bash
pip install -r requirements.txt
