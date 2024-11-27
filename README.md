# Document_Similarity_with_BERT
# Document Similarity with BERT

This project demonstrates the use of pre-trained BERT models and other deep learning techniques to compute document similarity, summarize text, and train/evaluate a semantic similarity classifier.

---

## **Requirements**

Before running the code, ensure you have the following dependencies and datasets set up.

### **Python Version**
- Python 3.8 or later

### **Required Python Packages**
Install the following Python packages:
```bash
pip install -U sentence-transformers transformers scikit-learn torch pandas gdown 
```

# Setup and Instructions

## 1. Datasets

The project uses the following datasets, which are automatically downloaded by the code:

- **Synthetic Dataset**:
    - URL: [Synthetic Data](https://github.com/Afag-Ramazanova/Document_Similarity_with_BERT/blob/main/dataset/Synthetic/synthetic_data2.csv)

- **Semantic Textual Similarity Benchmark (STS)**:
    - Training set: `stsbenchmark_train.csv`
    - Validation set: `stsbenchmark_validation.csv`
    - Test set: `stsbenchmark_test.csv`

No manual setup is required for datasets.

## 2. Pre-trained Models

The project uses the following models:

- **BERT** (`bert-base-uncased`): For embeddings and classification tasks.
- **BART** (`facebook/bart-large-cnn`): For summarization.
- **SentenceTransformer** (`sentence-transformers/bert-base-nli-mean-tokens`): For summarizing embeddings and computing similarity.

These models are automatically downloaded during runtime. Ensure an active internet connection for the initial run.

## 3. Saved Model for Inference

Download the trained BERT model (`finalized_model.pth`) using the `gdown` library:

```bash
gdown https://drive.google.com/uc?id=1F6xWrYqsGD-o8eSwIbUedLmtSoNNfhVv ```
```
## 4. Running the Code

- Clone the repository or ensure the scripts are in your working directory.
- Execute the code in a Python environment (e.g., Jupyter Notebook, VSCode, or terminal).
- Follow the instructions in the code to train, evaluate, and infer results.

---

## Special Notes

- Ensure you have GPU support for faster training and inference.
- The `gdown` library simplifies downloading from Google Drive. Ensure the file ID matches the one provided above.
- Internet access is required to download pre-trained models during the first run.

---

## License

This project uses open-source datasets and models. Please ensure compliance with respective licenses for Hugging Face and dataset sources.

