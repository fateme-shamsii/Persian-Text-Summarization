# Persian Text Summarization with Transformers (pn_summary)

This project focuses on automatic summarization of Persian news articles using transformer-based models. The goal is to train a model capable of generating human-like summaries for long Persian texts, using the [pn_summary](https://huggingface.co/datasets/HooshvareLab/pn_summary) dataset.

---

## 🎯 Objective

This project aims to provide hands-on experience with the complete pipeline of text summarization in Persian using transformer models:

- Load and explore the pn_summary dataset
- Preprocess and tokenize articles and summaries
- Fine-tune a text-to-text model for summarization
- Evaluate the model using ROUGE metrics
- Analyze results and suggest improvements

---

## 📚 Dataset: pn_summary

- **Source**: HooshvareLab
- **Total Samples**: 93,207 news articles
- **Fields**:
  - `article`: the original news content (input to the model)
  - `summary`: human-written summary (target output)
- 📎 [Dataset link](https://huggingface.co/datasets/HooshvareLab/pn_summary)

---

## 🧠 Model

We use a pre-trained text-to-text transformer model that supports the Persian language, such as:

- `HooshvareLab/bert2bert-fa`
- `mT5-small` or `mT5-base`

The model is fine-tuned to take the `article` as input and generate a summary resembling the human-written `summary` field.

