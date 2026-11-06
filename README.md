# Stance Detection on Bangla Climate News with LLMs

> 🚧 **This is an ongoing project.** Notebooks and methods will be added as the work progresses.

Classifying the stance of Bangla climate and environmental news articles using prompt-based LLM classification on the [Dhoroni](https://huggingface.co/datasets/ciol-research/Dhoroni) dataset.

## Task

Each article (title + first 1,200 characters of body) is labelled with one of four stances from the dataset's `Stance Detection` column:

- **Positive**
- **Negative**
- **Neutral**
- **Problematic**

## Notebooks

| Notebook | Method | Model |
|---|---|---|
| `main.ipynb` | Zero-shot prompting | Qwen2.5-3B-Instruct |

## Notebook Contents

1. Dataset exploration (label distributions, text lengths, label associations via Cramér's V)
2. Loading labels and article text from Hugging Face
3. Building a stratified evaluation sample
4. Zero-shot prompting and inference
5. Evaluation (accuracy, classification report, confusion matrix, error examples)

## Requirements

```bash
pip install transformers datasets scikit-learn pandas matplotlib seaborn huggingface_hub
```

A GPU is recommended (tested on Google Colab, T4).

## Dataset

[ciol-research/Dhoroni](https://huggingface.co/datasets/ciol-research/Dhoroni) — Bangla climate and environmental news articles with multiple annotation columns.

## Contact

iffathoque0@gmail.com
