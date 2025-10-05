# Pre-train Hugging Face

## Project Overview
This repository gathers reproducible resources for experimenting with Hugging Face Transformers on commodity hardware. It pairs two complementary notebooks with the raw WikiText dataset so that collaborators can explore both inference and continued pre-training workflows end-to-end.

## Repository Structure
- `Loading Models and Inference with Hugging Face.ipynb` - documents a publication-ready inference guide covering manual and `pipeline()`-based sentiment analysis with DistilBERT, GPT-2 text generation, and BERT mask filling on CUDA-enabled machines.
- `Optional Pre-training LLMs with Hugging Face.ipynb` - demonstrates how to resume language-model pre-training using Hugging Face Transformers, including environment setup, tokenizer/model configuration, and evaluation checkpoints.
- `wikitext_dataset_train.txt` / `wikitext_dataset_test.txt` - provide the WikiText corpus used throughout the notebooks for experimentation and benchmarking.

## Usage
1. Create and activate a Python 3.13+ virtual environment with PyTorch and Transformers installed.
2. Open either notebook in JupyterLab or VS Code and follow the sequenced cells. The inference notebook walks through model loading, tokenisation, and decoding, while the pre-training notebook drives masked language modelling on WikiText.
3. Adjust hyperparameters, prompts, or dataset slices to extend experiments and record findings in new commits.

## Contribution Guidelines
- Keep notebooks executable from top to bottom; re-run before committing to ensure outputs align with the documented narrative.
- Store additional datasets in dedicated subdirectories and reference them clearly from notebook metadata.
- Prefer pull requests for substantive changes so reviewers can validate results and maintain project quality.
