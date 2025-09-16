📝 **BERT-Sum: Extractive Text Summarization**
📌 Overview
This project implements an extractive text summarization system using BERT and Sentence-BERT (SBERT). The model identifies the most relevant sentences from a document to generate concise and informative summaries. Unlike abstractive summarization, extractive methods ensure factual accuracy by selecting original sentences.

📊 **Dataset**
BBC News Summary Dataset
Preprocessed into sentence-level units.
Weak supervision via ROUGE scoring used to label sentences as “summary-worthy.”

⚙️** Methodology**

**Sentence Embedding:**
Fine-tuned BERT and SBERT to encode sentences.
**Label Generation:**
Computed ROUGE overlap between candidate sentences and reference summaries.
**Classification Model:**
Built a classifier to predict whether a sentence should be included in the summary.
Selected top-k sentences based on predicted relevance.
**Evaluation:**
Benchmarked with ROUGE scores and classification metrics (accuracy, F1).

🚀 **Results**

Achieved higher ROUGE scores compared to baseline extractive methods (TF-IDF, TextRank).

Automated preprocessing, training, and evaluation pipeline for scalability.

🛠️ **Tech Stack**

Python, Transformers (Hugging Face), Scikit-learn, NLTK

BERT, SBERT

Evaluation: ROUGE, Accuracy, Loss
