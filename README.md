# Fake News Detection NLP

This project focuses on building a Fake News Detection system using advanced Natural Language Processing (NLP) techniques. By leveraging the Word2Vec model and multiple supervised learning algorithms—including Logistic Regression, Decision Tree, and Random Forest classifiers—the system classifies news articles as either true or fake based on their textual content. The project not only explores data cleaning, preprocessing, and exploratory data analysis but also compares the performance of different machine learning models to determine the most accurate and efficient approach. This solution aims to combat misinformation by providing an automated, reliable tool for news verification.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- **Problem Statement:**<br>
The spread of fake news has become a significant challenge in today’s digital world. With the massive volume of news articles published daily, it’s becoming harder to distinguish between credible and misleading information. This creates a need for systems that can automatically classify news articles as true or fake, helping to reduce misinformation and protect public trust.
- **Objective:**<br>
The objective of this project is to develop a Semantic Classification model that employs the Word2Vec method to identify recurring patterns and themes in news articles. The goal is to build a system using supervised learning models to classify news articles as either fake or true.
- **Methodology / Techniques Used:**<br>
The methodology followed in this project involves several key steps to build and evaluate a model for classifying news articles as either fake or true.<br>
  **1. Data Preparation:** The data preparation phase involved adding new columns to the dataset, merging DataFrames, and handling null values. Relevant columns were then merged to ensure the dataset was ready for analysis.<br>
  **2. Text Preprocessing:** Text cleaning was performed to remove unnecessary characters and noise. This was followed by part-of-speech (POS) tagging and lemmatization to standardize and reduce the words to their base form, ensuring consistency across the dataset.<br>
  **3. Train-Validation Split:** The data was split into training and validation sets using a 70:30 ratio to ensure a balanced and unbiased evaluation of the models.<br>
  **4. Exploratory Data Analysis (EDA):** EDA on the training data included visualizing the character lengths of the cleaned and lemmatized news text with POS tags removed, identifying and displaying the top 40 words by frequency, and analyzing the top unigrams,                bigrams, and trigrams in both true and fake news. These insights helped in understanding the distribution of key terms within the dataset.<br>
  **5. Feature Extraction:** The Word2Vec model was initialized, and vectors were extracted from the cleaned news data. This was critical in capturing semantic relationships between words for better feature representation.<br>
  **6. Model Training and Evaluation:** Three different models—Logistic Regression, Decision Tree, and Random Forest—were built and trained on the data. Each model was evaluated for its performance on the training set and tested against the validation set. The models'          metrics, such as accuracy, precision, recall, and F1 score, were used to assess and compare their effectiveness in classifying news articles.<br>
 - **Data Cleaning:**<br>
The text data was cleaned using a structured set of functions to ensure it was consistent and suitable for model training. The clean_text function was first applied to convert all text to lowercase, remove square bracketed content, eliminate punctuation, and discard words containing numbers. Following this, the find_weird_characters function was used to identify rows containing non-standard or special characters. This check revealed that 25,504 rows contained such characters, with unique weird characters like é, ™, •, ñ, €, ツ, ☑, ➡, and many others. These characters, which are often problematic for NLP models, were removed using the clean_weird_characters function. This function used a regular expression pattern to retain only standard alphanumeric characters and basic punctuation, ensuring the cleaned text was well-formatted and free of unwanted noise.
- **POS Tagging and Lemmatization:**<br>
A function named lemma_pos_tag was created to generate lemmatized words along with their POS (Part-of-Speech) tags for each word in the corpus. The nlp function from the spaCy library was used to perform this task. A new column was added to the dataset to store the combination of lemmatized words and their POS tags. Additionally, another column containing only the lemmatized words was created for use in further analysis. After completing all the preprocessing steps, the cleaned and processed dataset was saved as a file named “Clean_df.csv” in the local directory. This was done to avoid repeating the preprocessing steps, allowing the CSV file to be reused directly for future analysis in this case study.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Conclusion 1 from the analysis
- Conclusion 2 from the analysis
- Conclusion 3 from the analysis
- Conclusion 4 from the analysis

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- library - version 1.0
- library - version 2.0
- library - version 3.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!
