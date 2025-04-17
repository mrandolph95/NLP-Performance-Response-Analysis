
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

- 27,000+ comments from Beyoncé’s 2016 Super Bowl performance
- 134,000+ comments from Kendrick Lamar’s 2025 Super Bowl performance
- Collected using the YouTube API (no personal data retained)

## Methodology

1. **YouTube Comment Scraping**
2. **No Preprocessing** (to evaluate tool behavior on raw data)
3. **Language Detection Models**: langid, langdetect, Langua
4. **Initial Sentiment Classification**: `cardiffnlp/twitter-roberta-base-sentiment`
5. **Manual Annotation**: 1,200 comments with culturally-aware guidelines
6. **Active Learning Loop**:
    - Select low-confidence predictions
    - Manually annotate
    - Retrain model
7. **Evaluation**:
    - Accuracy, error types, misclassified examples
    - Focus on model errors involving emojis and informal expressions

## Key Findings

- Popular language detection tools frequently misclassified English comments as foreign when AAVE-derived or emoji-heavy language was used.
- Sentiment models misinterpreted slang and emojis, labeling positive expressions as negative or neutral.
- Manual annotation and active learning significantly improved the performance of sentiment classification on informal internet language.

## Responsible AI & Cultural Awareness

This research emphasizes the need for dialectally diverse datasets and culturally-aware annotation practices. It shows that treating internet language as "noise" leads to biased model behavior and digital exclusion.

## How to Use

_Notebooks and sample data coming soon._

## Author

Malachi Randolph  
malirandolph@yahoo.com


