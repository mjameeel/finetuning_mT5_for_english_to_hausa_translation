# Fine-Tuning mT5 for English–Hausa Translation

This repository contains an end-to-end implementation of **fine-tuning the multilingual T5 (mT5) model for English to Hausa machine translation**, along with a simple **Streamlit web application** for inference.

The project demonstrates how to prepare a bilingual dataset, fine-tune a pretrained sequence-to-sequence transformer using the Hugging Face ecosystem, and deploy the resulting model for real-world usage.

---

## 📌 Project Overview

- **Task:** Neural Machine Translation (English → Hausa)
- **Model:** `google/mt5-small`
- **Frameworks:** Hugging Face Transformers, Datasets, PyTorch
- **Execution Environment:** Google Colab (Free GPU)

This project is particularly relevant for **low-resource language translation** and can be extended to other African or multilingual NLP tasks.

---

## 🧠 Key Features

- End-to-end fine-tuning of an mT5 model
- Dataset preparation and sampling
- Tokenization for sequence-to-sequence learning
- Model training and inference
- Translation of unseen English sentences

---

## 📂 Repository Structure

├── Finetunining_mT5.ipynb # Main notebook (training + inference)
├── requirements.txt # Project dependencies
├── translation.jpg # Project illustration
└── README.md # Project documentation

---

## 📊 Dataset

- **Source:** English–Hausa parallel corpus from Kaggle
- **Format:** CSV (`en-ha.csv`)
- **Preprocessing Steps:**
  - Removal of unnecessary columns
  - Random sampling for efficient training
  - Conversion to Hugging Face `Dataset` object

The dataset is loaded programmatically using `kagglehub` and prepared for transformer-based training.

---

## ⚙️ Environment Setup

The project is designed to run seamlessly on **Google Colab** with GPU acceleration.

### Install Dependencies
```bash
pip install -U transformers datasets sentencepiece accelerate kagglehub

---

## 🚀 Future Improvements

- Train on larger and more diverse datasets

- Add BLEU / chrF evaluation metrics

- Deploy using Hugging Face Spaces or Docker

- Extend to bidirectional translation (Hausa ↔ English)

- Experiment with larger mT5 variants

---

## ⭐ Acknowledgements

- Google Research (mT5)

- Hugging Face 🤗

- Kaggle Datasets

---

## 👤 Author

Muhammad Jamil Abdulhamid
Data Scientist | Machine Learning Practitioner
Focus: NLP, Low-Resource Languages, Applied AI
