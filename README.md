# Multi-Document News Summarization (Indian English)

This repository contains the implementation, experiments, and evaluation results
for a multi-document abstractive news summarization project focused on
Indian English news articles.

We benchmark and analyze three transformer-based models on long,
multi-document inputs:

- **BART**
- **PEGASUS**
- **LED (Longformer Encoder-Decoder)**

---

## Repository Structure

newssummsummarization/
├── notebooks/ # Training, inference, and evaluation notebooks
├── results/ # ROUGE scores and generated summaries
├── .gitignore # Excludes large datasets
└── README.md


---

## Models Used

- **BART**  
  Encoder–decoder transformer used as a strong baseline for abstractive summarization.

- **PEGASUS**  
  Pretrained using gap-sentence generation, designed specifically for summarization tasks.

- **LED (Longformer Encoder-Decoder)**  
  Supports long-sequence inputs using sparse attention, making it suitable for
  multi-document summarization.

---

## Dataset

The dataset used in this project consists of Indian English news articles and
their corresponding human-written summaries.

📦 **Public Dataset Download (Google Drive):**  
**PASTE_DRIVE_LINK_HERE**

---

## Dataset Setup (IMPORTANT)

After downloading the dataset from Google Drive:

1. Extract the folder.
2. Place it in the project root directory with the following structure:

data/
├── raw/ # Original dataset files
├── processed/ # Preprocessed CSV files


⚠️ The `data/` directory is intentionally excluded from GitHub due to file size
limitations and must exist **locally** for the notebooks to run.

---

## Reproducibility Instructions

Follow these steps to reproduce the experiments:

1. Clone the repository:
   ```bash
   git clone https://github.com/saurabhhumane125/newssummsummarization.git
   cd newssummsummarization
