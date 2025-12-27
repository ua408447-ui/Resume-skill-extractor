# 🚀 AI Resume Skill Extractor (NER)

An automated system to extract key information from resumes using **Named Entity Recognition (NER)**. This project fine-tunes a **BERT-base-cased** model to identify skills, experience, and education from raw resume text.

## 🌟 Features
* **Deep Learning Engine:** Fine-tuned BERT-base model for high-accuracy entity extraction.
* **Extended Context:** Supports up to 512 tokens to capture data from long resumes.
* **Hybrid Extraction:** Combines Neural Networks with a keyword safety net for maximum reliability.
* **Interactive UI:** Built-in Gradio web interface for real-time testing.
* **Colab Optimized:** Includes mixed-precision (FP16) training for fast execution on T4 GPUs.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Hugging Face Transformers, Datasets, PyTorch, Seqeval
* **Model:** `bert-base-cased`
* **Interface:** Gradio
* **Environment:** Google Colab / Jupyter Notebook

## 📊 Model Performance
The model was fine-tuned using a BIO-tagging (Beginning, Inside, Outside) format. 
* **Epochs:** 15 (with Early Stopping)
* **Learning Rate:** 2e-5
* **Batch Size:** 8
* **Optimizer:** AdamW with Warmup

## 🚀 How to Use

### 1. Installation
```bash
pip install transformers datasets evaluate seqeval gradio torch
