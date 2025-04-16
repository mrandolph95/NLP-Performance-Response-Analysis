# Sentiment Analysis of YouTube Comments on Political Themes and the Black Experience

This project focuses on sentiment analysis of YouTube comments from two music performances that explore political themes and the Black experience in America. The goal is to classify comments as positive, neutral, or negative and analyze the sentiment expressed in these comments. The project incorporates responsible AI principles and includes advanced techniques such as handling emojis in sentiment analysis.

## Project Structure

The project is organized into the following main scripts:
	1.	**Data Preprocessing**
	•	Prepares the YouTube comments data by cleaning and normalizing the text.
	•	Includes steps for tokenization, stopword removal, and handling emojis.
	2.	**Sentiment Labeling**
	•	Self-labels a subset of the dataset based on predefined guidelines.
	•	Prepares the data for training by organizing it into sentiment categories (positive, negative, neutral).
	3.	**Model Training**
	•	Trains a sentiment analysis model using a pre-trained model (e.g., BERT) or custom classifier.
	•	Includes steps for splitting the data, training the model, and evaluating its performance.
	4.	**Model Evaluation**
	•	Evaluates the trained model on a test set, providing metrics like accuracy, precision, recall, and F1-score.
	•	Generates visualizations of model performance (e.g., confusion matrix).
	5.	**Visualization**
	•	Generates various visualizations such as sentiment distribution across comments, word clouds, and sentiment analysis insights.

## Requirements

To run this project, you will need to install the following dependencies:
	•	Python 3.x
	•	Pandas
	•	Numpy
	•	Scikit-learn
	•	Matplotlib
	•	Seaborn
	•	Transformers (for pre-trained models like BERT)
	•	TensorFlow or PyTorch (depending on which framework you use for model training)

You can install these dependencies by running:

pip install -r requirements.txt

## Dataset

The dataset consists of YouTube comments from two music performances that explore political themes and the Black experience in America. The comments are collected using the YouTube API (or scraped using a custom script).

## Responsible AI Considerations

This project takes responsible AI principles into account by:
	•	Ensuring fairness in sentiment classification.
	•	Handling potential biases in the dataset.
	•	Incorporating techniques for analyzing and mitigating bias in model predictions.
