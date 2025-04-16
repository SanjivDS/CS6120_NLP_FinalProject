# 🧠 Automated Critique & Review System using LLMs

This project implements an end-to-end pipeline for automated academic paper critique using Large Language Models. Given a PDF research paper, the system performs:

- 📄 Section-wise summarization
- ✍️ Paragraph-level critique generation using a fine-tuned Mistral model
- ⚖️ Bias detection using sentiment analysis (VADER)
- 📋 Plagiarism detection using embedding similarity with PeerRead dataset

---

## 🔍 Features

- **PDF Parsing:** Extracts and splits papers into structured sections and paragraphs
- **Summarization:** Generates concise section summaries using BART
- **Critique Generation:** Calls a Hugging Face API to get peer-review style feedback
- **Bias & Plagiarism Flags:** Paragraphs are evaluated for potential bias and plagiarism
- **Data Source:** Evaluation uses real abstracts from the PeerRead dataset

---

## 🚀 How to Run

### 1. Upload PDF
Run the notebook and upload any research paper in `.pdf` format.

### 2. Install Dependencies
Make sure to install all the required packages (see below or `requirements.txt`).

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
