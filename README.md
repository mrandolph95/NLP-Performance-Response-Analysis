
# When Sentiment Models Misread Internet Language

This project analyzes how NLP models misinterpret culturally expressive internet language—particularly informal YouTube comments that use emojis and slang—due to a lack of training on dialectally diverse and non-standard English inputs.

## Overview

Modern NLP tools often mislabel or misinterpret internet language that blends cultural slang, emojis, and non-standard grammar. Phrases like “slay,” “queen,” and emoji expressions such as the skull (💀) often carry positive sentiment but are misclassified as negative. This project explores how sentiment and language detection models fail on such data, using a real-world case study of YouTube comments from two music performances.

## Objectives

- Evaluate the accuracy of language detection tools on raw, internet-style English comments.
- Assess how transformer sentiment models classify culturally expressive and emoji-heavy content.
- Use manual annotation and active learning to improve classification performance.
- Highlight responsible AI considerations and ethical annotation practices.

## Dataset

- `beyonce_sample.csv`: Sample of comments from Beyoncé’s 2016 Super Bowl performance
- `kendrick_sample.csv`: Sample of comments from Kendrick Lamar’s 2025 Super Bowl performance
- Collected using the YouTube API (see `scraping.ipynb`)

## Repository Structure

- `scraping.ipynb`: Code for collecting YouTube comments
- `language_identification.ipynb`: Evaluation of langid, langdetect, and Langua
- `sentiment_model.ipynb`: Sentiment analysis using `cardiffnlp/twitter-roberta-base-sentiment`
- `active_learning.ipynb`: Low-confidence sampling and iterative retraining
- `annotation_guidelines.md`: Definitions and examples for sentiment labels
- `pipeline.png`: Visual diagram of the project workflow
- `language_missclassification_examples.pdf`: Sample errors from language detection models
- `sentiment_missclassification_examples.pdf`: Sample errors from sentiment classification
- `poster.pdf`: Research poster

## Methodology

1. **YouTube Comment Scraping**
2. **No Preprocessing** (to evaluate tool behavior on raw data)
3. **Language Detection Models**: langid, langdetect, Langua
4. **Initial Sentiment Classification**: `cardiffnlp/twitter-roberta-base-sentiment`
5. **Manual Annotation**: 1,200 comments using culturally-aware guidelines
6. **Active Learning Loop**:
    - Select low-confidence predictions
    - Manually annotate
    - Retrain model
7. **Evaluation**:
    - Accuracy, error types, misclassified examples (see PDFs)
    - Focus on model errors involving emojis and informal expressions

## Key Findings

- Language detectors often misclassified internet language as non-English, particularly short, emoji-heavy phrases.
- Sentiment models frequently misread slang and emojis, e.g., interpreting “she ate” or “💀” as negative.
- Active learning improved classifier performance by focusing manual effort on ambiguous comments.

## Responsible AI & Cultural Awareness

This research emphasizes the need for dialectally diverse datasets and culturally-aware annotation practices. It shows that treating internet language as "noise" leads to biased model behavior and digital exclusion.

## Author

Malachi Randolph  
malirandolph@yahoo.com

## License

This project is licensed under the MIT License.
