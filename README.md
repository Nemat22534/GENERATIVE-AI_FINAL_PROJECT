# English to Russian Translation using MarianMT

This project is part of the Generative AI course final assignment by **Nemat Dadashov (Student No: 210208749)**. It demonstrates a simple machine translation system using the MarianMT model, fine-tuned on the `opus_books` English-Russian dataset.

---

## Project Objective

The aim of the project is to build a working translator that can convert English text into Russian using a pre-trained transformer-based model and apply **fine-tuning** to improve translation quality.

---

## Model

- **Base Model**: Helsinki-NLP/opus-mt-en-ru
- **Technique**: Fine-tuning on a subset of the `opus_books` dataset
- **Framework**: Hugging Face Transformers & Datasets
- **Platform**: Google Colab

---

## How It Works

1. Load the MarianMT pre-trained model and tokenizer.
2. Load and preprocess the `opus_books` dataset (English–Russian translation).
3. Fine-tune the model on 1000 training samples and validate on 200 samples.
4. Use a translation pipeline to test the model with English sentences.

---

## Requirements

Install dependencies using:

```bash
pip install transformers datasets
