YouTube Comment Analysis for a Mumbai-based Digital Marketing Agency
Project Overview
This project provides a comprehensive text analysis of YouTube comments, designed to extract actionable insights for a digital marketing agency in Mumbai. By applying Natural Language Processing (NLP) techniques, the script automates the process of cleaning raw comment data, performing sentiment analysis, identifying key discussion topics, and discovering significant n-gram phrases.

The primary goal is to help the agency understand audience sentiment, identify content themes that resonate most with viewers, and inform their content strategy with data-driven insights.

Key Features
Data Preprocessing: Cleans and normalizes raw text data by removing missing values, converting text to lowercase, and eliminating special characters and common English stopwords.

Sentiment Analysis: Categorizes each comment as 'Positive', 'Negative', or 'Neutral' and assigns a numerical sentiment score, providing a clear understanding of audience emotion.

Topic Modeling: Utilizes Non-Negative Matrix Factorization (NMF) to automatically discover and summarize the main topics being discussed within the comments.

N-Gram Analysis: Identifies and ranks the most frequent two-word (Bigrams) and three-word (Trigrams) phrases, revealing common expressions and linked concepts.

Word Cloud Generation: Creates a visual representation of the most prominent words for each discovered topic, offering an intuitive and engaging overview of the content.

Automated Output: Generates a new Excel file containing all processed data, including sentiment scores and categories, for easy access and further analysis.

Technologies Used
Python: The core programming language for the project.

pandas: For efficient data manipulation and Excel file handling.

nltk: A robust library for text tokenization and managing stopwords.

textblob: A simple yet powerful tool for sentiment analysis.

scikit-learn: Used for advanced text vectorization (TfidfVectorizer) and topic modeling (NMF).

matplotlib & wordcloud: For generating high-quality visualizations of the word clouds.

re: For regular expressions to handle special character removal.

Getting Started
Prerequisites
Ensure you have Python 3.x installed on your system.

Installation
Clone the repository:

Bash

git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
Install the required libraries:

Bash

pip install pandas nltk textblob scikit-learn wordcloud matplotlib
Download NLTK data:
Run the following commands once to download the necessary data for NLTK, which is crucial for the preprocessing steps.

Python

import nltk
nltk.download('punkt')
nltk.download('stopwords')
Usage
Place your dataset:
Ensure your input Excel file with the YouTube comments is named dataset yt comment exam.xlsx and is placed in the same directory as the Python script. The script assumes the comment column is titled comment.

Run the script:
Simply execute the Python file from your terminal.

Bash

python your_script_name.py
Project Output
Upon successful execution, the script will perform the following actions:

Generate two Excel files:

Genexam.xlsx: Contains the preprocessed and cleaned data.

Genexamresult.xlsx: The final output, which includes the original comments, the processed text, and the new sentiment_score and sentiment_category columns.

Print analysis to the console:

The top words for each of the 5 discovered topics.

The top 20 most common Bigrams and Trigrams.

Display visual word clouds:

A separate word cloud image will be displayed for each of the 5 topics, providing a quick visual summary.
