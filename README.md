
# Sentiment Analysis of YouTube Comments on Political Music Performances

This project explores sentiment in YouTube comments related to politically and socially conscious music performances by Beyoncé and Kendrick Lamar. The goal is to analyze public reactions to themes around the Black experience and assess how online discourse is shaped by race, politics, and performance.

## Overview

The project uses comments from the following performances:
- **Beyoncé at Coachella (2018)**
- **Kendrick Lamar at the Grammys (2016)**

The analysis is built on sentiment classification using logistic regression and BERT-based models. It also includes targeted data cleaning for emojis, slang, and noise in user-generated content.

## Objectives

- Assess how audiences react emotionally to Black cultural and political expression in mainstream media.
- Evaluate comment sentiment distribution across artists and platforms.
- Mitigate racial bias in sentiment prediction through careful dataset curation and modeling.

## Methodology

### 1. Data Collection
- YouTube comments scraped using the YouTube API.
- Data includes usernames, timestamps, like counts, and raw text.

### 2. Preprocessing
- Removal of stopwords, special characters, URLs.
- Handling of emojis via translation to text using the `emoji` Python package.
- Spelling correction and lowercasing.
- Manual and semi-automated labeling of a subset of comments (Positive, Negative, Neutral).

### 3. Modeling
- **Logistic Regression** for baseline.
- **BERT-based transformer model** (via HuggingFace) for improved performance and nuance.
- Evaluation using accuracy, F1-score, precision, and recall.

### 4. Bias Mitigation
- Analysis of model errors on race-related content.
- Adjustments using re-weighting of training samples and subgroup evaluation.

## Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Transformers)
- YouTube Data API
- Jupyter Notebook / Google Colab
- HuggingFace Transformers
- NLTK / SpaCy / Emoji

## Results Summary

- BERT achieved an F1-score of 0.81 vs 0.69 for logistic regression.
- Comments on Beyoncé’s performance showed higher rates of polarization.
- Emojis were significant sentiment cues (e.g., 💯, 😢, 👏).
- Initial bias detection found false positives labeling neutral or supportive comments as negative when referencing Black identity — reduced after mitigation.

## Potential Applications

- Tools for platform moderation.
- Media studies and social science research.
- Understanding cultural response and emotional triggers in digital discourse.

## Next Steps

- Expand dataset to more performances (e.g., Childish Gambino’s “This Is America”).
- Integrate named entity recognition (NER) for deeper content parsing.
- Train a custom sentiment classifier on culturally diverse datasets.

## Author

[Your Name]

---

For academic inquiries or collaboration: [your.email@example.com]
