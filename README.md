# 🧠 Fine-Tuning a Legal Domain LLM using LoRA (PEFT)

## 📌 Project Overview

This project demonstrates how to fine-tune a Large Language Model (LLM) using LoRA (Low-Rank Adaptation) for generating domain-specific responses in formal legal language.

The goal is to transform a general-purpose conversational model into a specialized legal assistant capable of answering legal questions with structured and professional responses.

---

## 🚀 Key Features

* Fine-tunes an open-source LLM using LoRA (PEFT)
* Uses a custom legal Q&A dataset
* Implements parameter-efficient training on Google Colab (GPU)
* Compares base model vs fine-tuned model outputs
* Generates structured, domain-specific responses

---

## 🧰 Tech Stack

* Python
* Hugging Face Transformers
* PEFT (LoRA)
* Datasets
* Google Colab (T4 GPU)

---

## 📥 Input

A dataset of legal question-answer pairs such as:

**Question:** What is a contract?
**Answer:** A contract is a legally enforceable agreement between two or more parties creating mutual obligations.

---

## 📤 Output

### 🔹 Before Fine-Tuning (Base Model)

* Generic and repetitive responses
* Lacks domain-specific tone

### 🔹 After Fine-Tuning

* Formal legal language
* Structured and context-aware responses
* Improved clarity and terminology

---

## 🧠 Key Concepts

### 🔹 Fine-Tuning

Adapting a pre-trained model to a specific domain using custom data.

### 🔹 LoRA (Low-Rank Adaptation)

A parameter-efficient technique that updates only a small subset of model weights instead of retraining the entire model.

### 🔹 PEFT

Parameter-Efficient Fine-Tuning reduces memory usage and training time.

---

## ⚙️ Workflow

1. Load pre-trained model (TinyLlama)
2. Create domain-specific legal dataset
3. Format data into chat-style prompts
4. Apply LoRA configuration using PEFT
5. Tokenize dataset and add labels
6. Train model using Hugging Face Trainer
7. Generate responses for evaluation
8. Compare base vs fine-tuned outputs

---

## 📊 Example

### Input:

What is a contract?

### Output (Fine-Tuned Model):

A contract is a legally enforceable agreement between two or more parties that establishes rights and obligations recognized by law.

---

## 📈 Results

The fine-tuned model demonstrates:

* Improved domain adaptation
* More formal and structured responses
* Better alignment with legal terminology

---

## 📂 Project Structure

```
legal-llm-finetuning/
│
├── legal_llm_finetuning.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---


