# Spam SMS Classification using SimpleKNN 📱🛡️

This project was developed as part of the Computer Science degree at **HIT (Holon Institute of Technology)**. 
The goal is to classify SMS messages as either **Spam** or **Ham** (legitimate) using a custom implementation of the K-Nearest Neighbors (KNN) algorithm and various Natural Language Processing (NLP) techniques.

## 👥 Authors
* **Lior Mashiah**
* **Golan Katzav**
* **Lotem Kimchi**
* **Eldad Simanian**

## 🚀 Project Overview
In this project, we explored the entire Machine Learning pipeline:
1. **Data Exploration & Cleaning**: Handling the SMS Spam Collection dataset, removing stopwords, and text normalization.
2. **Feature Engineering**: Implementing and comparing 4 different vectorization methods:
   * CountVectorizer (Bag of Words)
   * TF-IDF (Unigrams)
   * TF-IDF (Bigrams)
   * TF-IDF + TruncatedSVD (Dimensionality Reduction)
3. **Algorithm Implementation**: A custom-built `SimpleKNN` class implemented from scratch.
4. **Model Selection**: Using **Grid Search** with **5-Fold Stratified Cross-Validation** to find the optimal $K$ and feature set.
5. **Model Explainability**: Using **SHAP** values to interpret the model's decisions and identify key "Spam" words.

## 📊 Results Summary
* **Best Model**: TF-IDF with Bigrams and $K=9$.
* **Primary Metric**: F1-Macro (Selected due to class imbalance).
* **Final Performance**: ~0.88 F1-Score on the test set.

## 🛠️ Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/liorma6/Spam-Detection-NLP.git](https://github.com/liorma6/Spam-Detection-NLP.git)
