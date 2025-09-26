YouTube Comment Analysis for a Mumbai-based Digital Marketing Agency
Project Overview
This project provides a comprehensive text analysis of YouTube comments to extract valuable insights for a digital marketing agency in Mumbai. By leveraging Natural Language Processing (NLP) techniques, the project cleans and preprocesses raw comment data, performs sentiment analysis, discovers key topics, and identifies important n-gram phrases.

The goal is to help the digital marketing agency understand public perception, identify popular discussion themes, and inform content strategy based on audience feedback.

Key Features
Data Preprocessing: Cleans raw text data by removing missing values, converting text to lowercase, removing special characters, and eliminating common English stopwords.

Sentiment Analysis: Categorizes each comment as 'Positive', 'Negative', or 'Neutral' and assigns a numerical sentiment score using the TextBlob library.

Topic Modeling: Employs Non-Negative Matrix Factorization (NMF) to automatically discover and summarize the main topics of discussion within the comments.

N-Gram Analysis: Identifies and ranks the most frequent bigrams (two-word phrases) and trigrams (three-word phrases) to reveal common expressions and linked concepts.

Word Cloud Generation: Visualizes the most prominent words for each discovered topic, providing an intuitive and quick overview of the content.

Excel Output: Saves all processed data, including sentiment scores and categories, into a new Excel file for easy access and further analysis.

Technologies Used
Python: The core programming language for the project.

pandas: For data manipulation and handling the Excel file.

re: For regular expressions to remove special characters.

nltk: A powerful library for tokenization and managing stopwords.

textblob: A simple yet effective library for sentiment analysis.

scikit-learn: Used for the TF-IDF vectorization and NMF topic modeling.

matplotlib & wordcloud: For generating visualizations, specifically the word clouds.

Getting Started
Prerequisites
Python 3.x installed on your system.

Access to the necessary Python libraries.

Installation
Clone the repository:

Bash

git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
Install the required Python libraries:

Bash

pip install pandas nltk textblob scikit-learn wordcloud matplotlib
Download NLTK data:
Run the following Python code once to download the necessary data for NLTK.

Python

import nltk
nltk.download('punkt')
nltk.download('stopwords')
Usage
Place your dataset:
Ensure your Excel file with the YouTube comments is named dataset yt comment exam.xlsx and is located in the same directory as the script. The script assumes the comment column is named comment.

Run the Python script:

Bash

python your_script_name.py
The script will perform the analysis and automatically generate two Excel files in the same directory:

Genexam.xlsx: Contains the preprocessed data.

Genexamresult.xlsx: Contains the final sentiment analysis results.

It will also print the results of the topic modeling and n-gram analysis to the console and display the generated word clouds.

Project Structure
.
├── dataset yt comment exam.xlsx # Original input file
├── your_script_name.py         # The main script
├── Genexam.xlsx                # Intermediate output file (preprocessed data)
├── Genexamresult.xlsx          # Final output file (sentiment & topics)
└── README.md                   # This file
Results & Insights
The final Genexamresult.xlsx file provides a rich dataset for the digital marketing team to explore. They can filter comments by sentiment, analyze specific topics, and use the word clouds and n-gram lists to guide content creation. For example, if Topic #1 is about "video quality," the team can use the top words from that topic to create more targeted content.
