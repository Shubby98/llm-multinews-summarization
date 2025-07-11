# llm-multinews-summarization

This project fine-tunes the pre-trained `facebook/bart-base` model for abstractive summarization on the [Multi-News](https://github.com/Alex-Fabbri/Multi-News) dataset. The entire pipeline—from preprocessing to training and evaluation—is implemented in a single Jupyter notebook.

---

## 📌 Project Overview

- **Dataset**: Multi-News (multi-document news summarization)
- **Model**: `facebook/bart-base`
- **Task**: Abstractive Summarization
- **Metrics**: ROUGE, BLEU, BERTScore

---

## 🗂️ Files

| File/Folder                     | Description                       |
| ------------------------------- | --------------------------------- |
| `summarization_multinews.ipynb` | Main notebook containing all code |
| `results/`                      | Stores predictions and reference  |
| `assets/`                       | Sample summary outputs            |
| `config/`                       | Training Configs and Eval Results |
| `requirements.txt`              | Python dependencies               |
| `README.md`                     | This file                         |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Shubby98/llm-multinews-summarization.git
cd llm-multinews-summarization
```