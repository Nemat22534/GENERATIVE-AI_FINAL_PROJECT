# English to Russian Translation using MarianMT

This project is part of the **Generative AI course final project by **Nemat Dadashov (Student No: 210208749)**. It demonstrates a simple machine translation system using the MarianMT model, fine-tuned on the `opus_books` English–Russian dataset.

---

## Project Objective

The aim of the project is to build a working translator that converts English text into Russian using a pre-trained transformer-based model and apply **fine-tuning** to adapt it to a specific domain (literary texts).

---

## Model Information

- **Base Model**: [Helsinki-NLP/opus-mt-en-ru](https://huggingface.co/Helsinki-NLP/opus-mt-en-ru)
- **Fine-tuning Dataset**: `opus_books` (subset: 1000 training, 200 validation samples)
- **Model Type**: MarianMT (Transformer architecture)
- **Frameworks**: Hugging Face Transformers, Datasets
- **Platform**: Google Colab / Python

---

## How It Works

1. Load the MarianMT model and tokenizer.
2. Load and preprocess the `opus_books` English–Russian translation dataset.
3. Fine-tune the model with:
   - 1000 training examples
   - 200 validation examples
4. Create a Hugging Face `pipeline` for inference.
5. Translate new English sentences and compare outputs.

---

## Requirements

```bash
pip install
transformers
datasets
sacrebleu
sentencepiece
