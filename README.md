# AI/ML Assignment 7: Fine-Tuning LLM with LoRA

**Student Name:** Ermiyas H.
**Base Model:** DistilBERT (distilbert-base-uncased)  
**Dataset:** IMDb Movie Reviews (Sentiment Analysis)  
**Technique:** Parameter-Efficient Fine-Tuning with LoRA  
**Date:** November 2025

## Project Overview

This project demonstrates fine-tuning a pre-trained language model (DistilBERT) for sentiment analysis using Low-Rank Adaptation (LoRA).

## LoRA Configuration

| Parameter | Value |
|-----------|-------|
| **Rank (r)** | 8 |
| **Alpha** | 16 |
| **Dropout** | 0.1 |
| **Target Modules** | q_lin, v_lin |

## Final Evaluation Metrics

| Metric | Score |
|--------|-------|
| **Accuracy** | 88.20% |
| **F1-Score** | 0.8872 |

## Comparison with Baseline

| Model | Accuracy | Improvement |
|-------|----------|-------------|
| Baseline | 55% | - |
| Fine-Tuned (LoRA) | **88.20%** | **+60.4%** |

## Why LoRA Saves Computational Resources

LoRA achieves significant computational savings:

1. **Reduced Trainable Parameters:** Only ~0.3% of parameters need training
2. **Memory Efficiency:** 4x reduction in GPU memory usage
3. **Faster Training:** 2-3x faster than full fine-tuning
4. **Storage Efficiency:** Adapters are only 1-2MB per task

## Repository Structure
```
AI-ML-Assignment-7-LLM-FineTuning-LoRA/
├── llm_finetuning_lora.ipynb
├── requirements.txt
├── README.md
└── results/
```

## How to Run
```bash
conda create -n llm_finetuning python=3.10 -y
conda activate llm_finetuning
pip install -r requirements.txt
jupyter notebook
```

## YouTube
[Link](https://youtu.be/_QaASatX-Yg)

## Key Learnings

- LoRA enables fine-tuning on modest hardware
- Achieved 60.4% accuracy improvement over baseline
- 99.7% reduction in trainable parameters

## Video Demonstration

[YouTube Link - to be added]
# AI-ML-Assignment-7-LLM-FineTuning-LoRA
