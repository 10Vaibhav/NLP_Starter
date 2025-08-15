# NLP Environment Setup

This repository contains code and environment setup for Natural Language Processing (NLP) projects. Follow the instructions below to set up your development environment.

## Quick Start

### 1. Create and Activate Conda Environment
```bash
# Create virtual environment with Python 3.11
conda create --name nlp_env python=3.11

# Activate the environment
conda activate nlp_env
```

### 2. Install Required Packages
```bash
# Install core NLP packages
pip install nltk==3.9.1 pandas==2.2.3 matplotlib==3.10.0 spacy==3.8.3 textblob==0.18.0.post0 vaderSentiment==3.3.2 transformers==4.47.1 scikit-learn==1.6.0 gensim==4.3.3 seaborn==0.13.2 torch==2.5.1 ipywidgets==8.1.5

# Download spaCy language model
python -m spacy download en_core_web_sm

# Install Jupyter components
pip install ipykernel jupyterlab notebook

# Register the environment as a Jupyter kernel
python -m ipykernel install --user --name=nlp_env
```

### 3. Launch Jupyter
```bash
jupyter lab
# or
jupyter notebook
```

**Important:** Make sure to select the `nlp_env` kernel when working with notebooks.

## Installed Packages

| Package | Version | Purpose |
|---------|---------|---------|
| `nltk` | 3.9.1 | Natural language processing toolkit |
| `pandas` | 2.2.3 | Data manipulation and analysis |
| `matplotlib` | 3.10.0 | Plotting and visualization |
| `spacy` | 3.8.3 | Industrial-strength NLP library |
| `textblob` | 0.18.0.post0 | Simple text processing |
| `vaderSentiment` | 3.3.2 | Sentiment analysis tool |
| `transformers` | 4.47.1 | Hugging Face transformer models |
| `scikit-learn` | 1.6.0 | Machine learning library |
| `gensim` | 4.3.3 | Topic modeling and word embeddings |
| `seaborn` | 0.13.2 | Statistical data visualization |
| `torch` | 2.5.1 | PyTorch deep learning framework |
| `ipywidgets` | 8.1.5 | Interactive Jupyter widgets |


## Environment Management

### Activating the Environment
```bash
conda activate nlp_env
```

### Deactivating the Environment
```bash
conda deactivate
```

### Removing the Environment (if needed)
```bash
conda remove --name nlp_env --all
```

### Listing Available Kernels
```bash
jupyter kernelspec list
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
