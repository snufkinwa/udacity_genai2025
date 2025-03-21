# Lightweight Fine-Tuning with LoRA (PEFT Project)

This project demonstrates how to apply parameter-efficient fine-tuning (PEFT) using LoRA (Low-Rank Adaptation) on a sequence classification task with a Hugging Face transformer model.

## 🧠 Project Overview

- **Model:** `distilbert-base-uncased`
- **PEFT Technique:** LoRA (Low-Rank Adaptation)
- **Dataset:** IMDb movie reviews (binary sentiment classification)
- **Evaluation:** Hugging Face `Trainer` + `evaluate` library

The goal was to:

1. Load a pre-trained model and evaluate it on a downstream task
2. Apply LoRA for parameter-efficient fine-tuning
3. Evaluate and compare the fine-tuned model’s performance

## 📋 Results

- We achieved an improvement in classification accuracy after fine-tuning using LoRA, while keeping the number of trainable parameters low.
- Inference examples demonstrate the fine-tuned model correctly identifying sentiment in movie reviews.

## 📁 Files

- `LightweightFineTuning.ipynb`: The complete notebook with training, evaluation, and inference steps.

## 🧪 How to Run

1. Clone this repo or open the notebook in a Jupyter environment.
2. Make sure the required libraries are installed:
   ```bash
   pip install transformers datasets peft evaluate
   ```
