cat << 'EOF' >> README.md

## Overview
This repository contains the implementation and evaluation of multi-document abstractive summarization models (BART, PEGASUS, and LED) trained and evaluated on Indian English news articles.

## Models
- BART (baseline encoder-decoder transformer)
- PEGASUS (pretrained with gap-sentence objective)
- LED (Longformer Encoder-Decoder for long multi-document inputs)

## Dataset Access

Due to GitHub file size limitations, the full NewsSumm dataset is not hosted in this repository.

📂 Dataset download link:
[Google Drive / Kaggle / Zenodo link]

The repository includes:
- Sample data for structure reference
- Preprocessing scripts
- Training and evaluation notebooks

This setup follows standard reproducibility practices used in large-scale NLP research.


## Experiments
- Training notebooks available in `notebooks/`
- Inference outputs and ROUGE scores available in `results/`

## Evaluation
- ROUGE-1, ROUGE-2, ROUGE-L computed on 25-document subset
- LED shows stronger structural and legal-context preservation

## Reproducibility
All experiments were conducted in Google Colab (Tesla T4 GPU).
Exact hyperparameters and training details are documented in notebooks.

EOF
