# Multilingual Sentiment Analysis and Lexicon Expansion for South African Languages

This project explores the development of a multilingual sentiment analysis tool for South African languages. It focuses on expanding an existing bilingual lexicon (French-Ciluba) to include English, Afrikaans, Zulu, Xhosa, and Sesotho and evaluates the effectiveness of various machine learning models for sentiment classification.

## Overview

South Africa's linguistic diversity presents unique challenges for sentiment analysis. This study addresses the underrepresentation of indigenous languages in NLP by:
- Expanding a lexicon to support sentiment classification in multiple languages.
- Applying machine learning models to classify sentiments across languages.
- Testing translation fidelity to maintain accurate sentiment interpretation.

### Key Features:
- **Languages Covered:** English, Afrikaans, Zulu, Xhosa, Sesotho, French, and Ciluba.
- **Machine Learning Models:** Random Forest, SVM, Logistic Regression, Decision Tree, and Naive Bayes.
- **Preprocessing Techniques:** SMOTE for class balancing, sentiment normalization, and translation validation (manual review and back-translation).
- **Evaluation Metrics:** Accuracy, F1 score, precision, recall, and ROC-AUC scores.

## Highlights of Results

- **Best Performing Model:** Random Forest achieved the highest accuracy and F1 scores, effectively capturing the complexity of multilingual data.
- **Translation Consistency:** Sentiment polarity and intensity were largely preserved across translations, with minor variations due to cultural and linguistic nuances.
- **Challenges:** Class imbalance, limited sentiment-rich adjectives in the lexicon, and difficulty in handling nuanced cultural expressions.

## Methodology

1. **Data Preparation:**
   - Cleaned and normalized text data.
   - Balanced sentiment classes using SMOTE.
   - Emphasized sentiment-rich parts of speech (e.g., adjectives).

2. **Model Training and Evaluation:**
   - Models were trained on the expanded lexicon.
   - Performance was evaluated using precision, recall, F1 scores, and ROC-AUC.

3. **Translation Testing:**
   - Translations were validated using back-translation and manual review to ensure fidelity.

## Observations and Challenges

- **Class Imbalance:** Despite using SMOTE, neutral sentiments were harder to classify due to limited data.
- **Cultural Nuances:** Some idiomatic expressions and emotional tones were difficult to translate accurately.
- **Model Limitations:** Simpler models (e.g., Logistic Regression and Naive Bayes) struggled with the nuanced multilingual dataset.

## Future Directions

- **Expand the Lexicon:** Include more culturally specific and sentiment-rich terms.
- **Advanced Models:** Explore deep learning approaches like transformers or attention-based models.
- **Diverse Datasets:** Incorporate social media, news, and informal text sources for better generalization.

## Usage

### Requirements
- Python 3.x
- Required libraries: NumPy, Pandas, Scikit-learn, and Matplotlib.

### Steps to Reproduce
1. Clone the repository:
   ```bash
   git clone https://github.com/MuhammadAyob/Multilingual-Sentiment-Analysis-Lexicon-Expansion.git
   cd multilingual-sentiment-analysis
