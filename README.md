
# Sentiment Analysis on YouTube Comments

This project showcases a sentiment analysis model applied to YouTube comments from music performances, particularly focusing on how language identification and sentiment models may fail to accurately analyze diverse dialects and expressions in online comments. The goal is to understand how models handle different types of speech patterns, sentiments, and biases when analyzing user-generated content.

## Overview

The project uses comments from the following performances:
- **Beyoncé & Bruno Mars Crash the Super Bowl 50 Halftime Show (2016)**
- **Kendrick Lamar’s Apple Music Super Bowl Halftime Show (2025)**

The analysis is built on sentiment classification using logistic regression and transformer-based models. It also includes targeted data cleaning for emojis, slang, and noise in user-generated content.

## Objectives

- Assess how audiences react emotionally to Black cultural and political expression in mainstream media.
- Evaluate comment sentiment distribution across artists and platforms.
- Mitigate cultural or dialect bias in sentiment prediction through careful dataset curation and modeling.

## Methodology

### 1. Data Collection
- YouTube comments scraped using the YouTube API.
- Data includes usernames, timestamps, like counts, and raw text.

### 2. Preprocessing
- Handling of emojis via translation to text using the `emoji` Python package.
- Manual and semi-automated labeling of a subset of comments (Positive, Negative, Neutral).

### 3. Modeling
- **Logistic Regression** for baseline.
- **Transformer-based transformer model** (via HuggingFace) for improved performance and nuance.

### 4. Bias Mitigation
- Analysis of model errors on dialectial-heavy comments.
- Adjustments using re-weighting of training samples and subgroup evaluation.

## Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Transformers)
- YouTube Data API
- Jupyter Notebook / Google Colab
- HuggingFace Transformers
- NLTK / Emoji

## Results Summary

- Emojis were significant sentiment cues (e.g., 💯, 😢, 👏).
- Initial bias detection found false positives labeling neutral or supportive comments as negative when using dialectal language.

## Potential Applications

- Tools for platform moderation.
- Media studies and social science research.
- Understanding cultural response and emotional triggers in digital discourse.

## Next Steps

- Use more human-annotators for sentiment review and human-in-the-loop sessions.
- Train a custom sentiment and language identification classifier on culturally diverse datasets.

## Author

Malachi Randolph

---

For academic inquiries or collaboration: malirandolph@yahoo.com
