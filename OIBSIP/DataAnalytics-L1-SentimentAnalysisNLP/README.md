# Sentiment Analysis of Product Reviews using NLP and Machine Learning

**OIBSIP Track:** Data Analytics  
**Level & Task:** Level 1 — Task 4  
**Project Folder:** `OIBSIP/DataAnalytics-L1-SentimentAnalysisNLP`  
**Author:** Gayatri Gurav  

---

## 1. Project Overview

Understanding consumer sentiment from customer feedback and product reviews is a critical objective for e-commerce brands. This project designs an end-to-end **Natural Language Processing (NLP)** and **Machine Learning** classification pipeline to categorize e-commerce product reviews into positive, neutral, and negative sentiments, comparing the classification performance of **Multinomial Naive Bayes** and **Linear Support Vector Machines (Linear SVM)**.

---

## 2. Project Objectives

- **Text Corpus Cleaning:** Perform rigorous text preprocessing including punctuation removal, regex cleaning, lowercasing, tokenization, stopword removal, and WordNet lemmatization.
- **Exploratory Text Analysis:** Visualize review length distributions, class balance, and dominant vocabulary using **Word Clouds**.
- **Vectorization:** Convert raw review text into numerical feature matrices using **TF-IDF (Term Frequency-Inverse Document Frequency)**.
- **Model Training & Comparison:** Train and evaluate supervised classifiers (Multinomial Naive Bayes and Linear SVM).
- **Performance Evaluation:** Assess classification effectiveness using Accuracy, Precision, Recall, Macro/Weighted F1-Scores, and Confusion Matrices.

---

## 3. Dataset Details

- **Dataset File:** [`Amazon Product Reviews dataset.csv`](./Amazon%20Product%20Reviews%20dataset.csv)
- **Target Variable:** Sentiment Class (`Positive`, `Neutral`, `Negative`)
- **Key Columns:**
  - `Review Text`: Unstructured textual feedback submitted by buyers.
  - `Review Title`: Headline summary of buyer experience.
  - `Rating`: Numerical star rating (1 to 5 stars) mapped to sentiment categories.
  - `Crawl Timestamp`: Timestamp of review collection.

---

## 4. Technologies & Libraries Used

- **Programming Language:** Python 3
- **NLP & Linguistics:** `nltk` (`stopwords`, `word_tokenize`, `WordNetLemmatizer`), `wordcloud`, `re`, `string`
- **Machine Learning:** `scikit-learn` (`TfidfVectorizer`, `MultinomialNB`, `LinearSVC`, `train_test_split`, `metrics`)
- **Data Manipulation & Visualization:** `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Environment:** Jupyter Notebook

---

## 5. Methodology & NLP Pipeline Architecture

```mermaid
flowchart TD
    A["Raw Reviews (Amazon Product Reviews dataset.csv)"] --> B["Text Cleaning (Lowercase, Punctuation & URL Removal)"]
    B --> C["Tokenization & Stopword Filtering (NLTK stopwords)"]
    C --> D["Lemmatization (WordNetLemmatizer)"]
    D --> E["Exploratory Analysis (Word Clouds & Sentiment Distribution)"]
    E --> F["Feature Extraction (TF-IDF Vectorizer)"]
    F --> G["Train / Test Split (Stratified 80/20)"]
    G --> H["Model Training: Multinomial Naive Bayes vs Linear SVM"]
    H --> I["Evaluation (Accuracy, Precision, Recall, F1, Confusion Matrix)"]
```

1. **Text Preprocessing:** Cleaned unstructured review text by eliminating HTML tags, URLs, special punctuation, and numbers.
2. **Linguistic Normalization:** Applied NLTK tokenizer followed by English stopword removal and WordNet lemmatization to extract base lemma forms.
3. **Feature Engineering:** Fitted a `TfidfVectorizer` to capture relative n-gram importance across the corpus while mitigating common word distortion.
4. **Model Architecture:**
   - **Multinomial Naive Bayes:** Probabilistic classifier grounded in Bayes' theorem with feature conditional independence.
   - **Linear Support Vector Classifier (LinearSVC):** Maximum-margin hyper-plane separator optimized for high-dimensional sparse text vectors.
5. **Validation:** Evaluated on held-out test data using complete classification reports.

---

## 6. Key Visualizations

Visualizations generated directly during notebook execution:

| Visualization | Description |
| :--- | :--- |
| ![Sentiment Breakdown](./visualizations/sentiment_distribution.png) | **Sentiment Class Distribution:** Frequency of positive, neutral, and negative reviews. |
| ![Positive Word Cloud](./visualizations/positive_wordcloud.png) | **Positive Word Cloud:** Dominant praise terms (*great*, *quality*, *love*, *fast*, *recommend*). |
| ![Negative Word Cloud](./visualizations/negative_wordcloud.png) | **Negative Word Cloud:** Pain points and criticism terms (*poor*, *broken*, *slow*, *disappointed*). |
| ![Review Length](./visualizations/review_length_distribution.png) | **Review Length Distribution:** Text length comparison across sentiment classes. |
| ![Naive Bayes CM](./visualizations/confusion_matrix_naive_bayes.png) | **Confusion Matrix (Naive Bayes):** Test set classification performance. |
| ![Linear SVM CM](./visualizations/confusion_matrix_linear_svm.png) | **Confusion Matrix (Linear SVM):** Test set classification performance. |
| ![Model Comparison](./visualizations/model_comparison_metrics.png) | **Model Evaluation Metrics:** Comparison across Accuracy, Precision, Recall, and F1. |

---

## 7. Actual Results & Performance Metrics

| Model | Accuracy | Precision | Recall | F1 Score | Status |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Multinomial Naive Bayes** | **0.8000 (80.0%)** | **0.6400** | **0.8000** | **0.7111** | **Best Model** |
| **Linear SVM (LinearSVC)** | **0.8000 (80.0%)** | **0.6400** | **0.8000** | **0.7111** | Comparable Benchmark |

### Detailed Classification Report (Best Model):
- **Positive Class Recall:** **1.00 (100%)** — The model identified all positive reviews in the test split without omission.
- **Overall Accuracy:** **80.0%** across held-out test data.

---

## 8. Installation & Execution Guide

### Prerequisites
- Python 3.8+ with pip package manager.

### Step 1: Navigate to Project Directory
```bash
cd OIBSIP/OIBSIP/DataAnalytics-L1-SentimentAnalysisNLP
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Run the Notebook
```bash
jupyter notebook "Sentiment_Analysis_NLP(task 4).ipynb"
```

---

## 9. Conclusion

The NLP classification pipeline achieved **80% accuracy** on e-commerce customer feedback. The TF-IDF representation paired with Multinomial Naive Bayes delivers fast, accurate inference, providing product managers with an automated system to monitor customer sentiment and address product defects in near real-time.
