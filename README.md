# pawonkoe-sentiment-analysis-mbert
Customer sentiment analysis for Pawonkoe using Multilingual BERT (mBERT), including text preprocessing, sentiment classification, model evaluation, word cloud visualization, and chi-square analysis.


# Pawonkoe Customer Sentiment Analysis using mBERT

This project focuses on analyzing customer sentiment toward Pawonkoe using **Multilingual BERT (mBERT)**, a transformer-based language model designed to process multilingual text.

The project applies text preprocessing and sentiment classification to customer feedback, followed by model evaluation and data visualization to help understand customer opinions and satisfaction.

## Project Objectives

- Analyze customer sentiment toward Pawonkoe.
- Classify customer feedback into sentiment categories.
- Evaluate sentiment classification performance.
- Visualize frequently occurring words in customer feedback.
- Explore the relationship between customer satisfaction ratings and predicted sentiment.

## Features

### 1. Text Preprocessing
Prepares customer feedback for sentiment classification through text cleaning, normalization, and label preparation.

### 2. Sentiment Classification with mBERT
Uses the pretrained `bert-base-multilingual-cased` model for customer sentiment classification.

### 3. Model Evaluation
Evaluates model performance using classification metrics, including accuracy, precision, recall, F1-score, and a confusion matrix.

### 4. Sentiment Visualization
Generates word clouds and other visualizations to explore patterns in customer feedback.

### 5. Customer Satisfaction Analysis
Uses a Chi-Square test and Cramer's V to examine the association between customer satisfaction ratings and predicted sentiment categories.

## Methodology

The project follows these main stages:

1. Load customer review and sentiment data.
2. Preprocess and prepare text data for model training.
3. Tokenize the text using the mBERT tokenizer.
4. Train and evaluate the sentiment classification model.
5. Generate sentiment predictions and extract model-related features.
6. Visualize sentiment patterns and evaluate classification results.
7. Analyze the relationship between satisfaction ratings and predicted sentiment.

## Model Configuration

| Component | Configuration |
|---|---|
| Pretrained model | `bert-base-multilingual-cased` |
| Model architecture | Multilingual BERT |
| Maximum sequence length | 128 tokens in the final training section |
| Training epochs | 5 |
| Number of sentiment classes | 3 |
| Main framework | PyTorch |
| Tokenization | Hugging Face Transformers |

## Technologies

- Python
- PyTorch
- Hugging Face Transformers
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- WordCloud
- SciPy

## Dataset

The notebook uses `Sentimen.xlsx` as its input dataset.

The dataset should contain the customer feedback and associated sentiment or satisfaction information required by the analysis.

**Note:** The original dataset is not included in this repository by default. Make sure you have permission to share any customer data before publishing it.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/USERNAME/pawonkoe-sentiment-analysis-mbert.git
cd pawonkoe-sentiment-analysis-mbert
```

### 2. Install dependencies

```bash
pip install pandas numpy torch transformers scikit-learn matplotlib seaborn wordcloud scipy openpyxl
```

### 3. Prepare the dataset

Place `Sentimen.xlsx` in the directory expected by the notebook, or update the dataset path in the code.

### 4. Run the notebook

Open `mbert_final.ipynb` using Jupyter Notebook, JupyterLab, or Google Colab and execute the cells in order.

The pretrained mBERT model and tokenizer may require an internet connection for their initial download unless they are already available locally.

## Output Files

The notebook is configured to generate or use the following files:

- `best_bert_model.pth` — saved model weights.
- `bert_tokenizer/` — saved tokenizer files.
- `sentiment_features_for_xgboost.csv` — sentiment predictions and extracted features used in subsequent analysis.

The notebook also produces evaluation reports, confusion matrix visualizations, word clouds, and Chi-Square analysis results.

## Project Information

- **Project Name:** PAISA — Pawonkoe Sentiment Analysis
- **Research Focus:** Customer Sentiment Analysis
- **Method:** Multilingual BERT (mBERT)
- **Research Context:** Pawonkoe, an UMKM business

## Disclaimer

This project is intended for academic research and customer feedback analysis. Model performance and analytical findings depend on the quality of the dataset and the training process.

---

**Turning Customer Feedback into Meaningful Insights.**
