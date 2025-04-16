
# Sentiment Analysis of YouTube Comments on Politically Themed Music Performances

This project explores the intersection of machine learning, natural language processing (NLP), and cultural analysis by examining public reactions to music performances by artists such as Beyoncé and Kendrick Lamar. These performances engage with political themes and the Black experience, and the goal is to analyze sentiment in the associated YouTube comments to understand patterns in reception and discourse.

## Project Objectives

- **Collect** YouTube comment data on culturally and politically significant music performances.
- **Preprocess** and clean the text data, including emoji handling and slang interpretation to preserve cultural nuance.
- **Label** sentiments accurately, addressing the challenges of informal language and potential annotation bias.
- **Build and compare** sentiment classification models (Logistic Regression, Naive Bayes, and BERT).
- **Mitigate bias**, particularly with regard to African American Vernacular English (AAVE), through lexicon analysis and dataset augmentation.
- **Visualize trends** in public sentiment over time and across different performance contexts.

## Technologies Used

- Python (Pandas, NumPy)
- NLP Libraries: NLTK, scikit-learn, Hugging Face Transformers
- YouTube Data API for data collection
- Jupyter Notebooks for exploratory analysis and modeling

## Highlights

- Custom emoji mapping and interpretation of informal language ensured culturally relevant sentiment extraction.
- BERT-based transformer models significantly outperformed traditional models in capturing sentiment from nuanced language.
- Incorporated ethical considerations in NLP by detecting and correcting potential model bias against AAVE.
- Analyzed patterns in public engagement with performances tackling race, politics, and identity.

## Future Work

- Expand dataset to include more artists and performances across genres.
- Improve model robustness by integrating additional social media platforms.
- Explore topic modeling to detect shifts in discourse related to social issues over time.

## How to Run

1. Clone this repository.
2. Install the dependencies listed in `requirements.txt`.
3. Use `run_model.py` to train or test models.
4. Notebooks in the `notebooks/` directory include data exploration and evaluation steps.

## Acknowledgements

Inspired by the intersection of music, activism, and cultural identity. Special thanks to the YouTube community for their unfiltered engagement with art.

---

*This project was created as part of a personal exploration into NLP, cultural data, and ethical machine learning.*
