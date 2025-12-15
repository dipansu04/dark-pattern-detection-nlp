# dark-pattern-detection-nlp
End-to-end NLP project for detecting dark patterns in website text using text preprocessing, TF-IDF features, and multiple machine learning classification models
# AI-Powered Dark Pattern Detection 🕵️‍♂️🚫

## Project Overview
This project uses Natural Language Processing (NLP) and Machine Learning to detect "Dark Patterns" in user interface text. Dark patterns are deceptive UI designs used to trick users into doing things they didn't mean to, like buying insurance or signing up for recurring bills.

This model classifies text into specific dark pattern categories (e.g., Urgency, Scarcity, Social Proof) with **94% accuracy**.

## Key Features
* **Text Preprocessing:** Automated pipeline for tokenization, stopword removal, and lemmatization.
* **Feature Engineering:** Utilized **TF-IDF Vectorization** (1-2 ngrams) to capture linguistic patterns.
* **Model Selection:** Benchmarked 5 algorithms (Logistic Regression, Naive Bayes, Random Forest, Linear SVM, Gradient Boosting).
* **Best Model:** **Linear Support Vector Machine (SVM)** achieved the highest accuracy (94.8%).
* **Hyperparameter Tuning:** Optimized using `GridSearchCV` (Best `C=10`).
* **Explainability:** Integrated **ELI5** to interpret model decisions and identify specific "trigger words" (e.g., "hurry," "limited," "offer") that signal deception.

## Dataset
* **Source:** `dark_patterns_dataset.csv`
* **Size:** ~2,300 labeled text samples.
* **Classes:** Urgency, Scarcity, Misdirection, Social Proof, Obstruction, Not Dark Pattern.

## Results
The tuned Linear SVM model achieved an accuracy of **94%** on the test set.

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 94% |
| **Precision** | 95% |
| **Recall** | 94% |
| **F1-Score** | 94% |

