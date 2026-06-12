# NLP-Text-Analytics-Pipeline
NLP Text Analytics Pipeline

Overview

This project is a comprehensive Natural Language Processing (NLP) analytics pipeline designed to extract meaningful insights from textual data such as news articles, reviews, and social media content. The system performs text preprocessing, topic modelling, sentiment analysis, named entity recognition, and visualizes results through an interactive dashboard.

The project demonstrates an end-to-end NLP workflow and can be applied to use cases such as competitive intelligence, customer feedback analysis, market trend monitoring, and news analytics.

---

Features

Text Preprocessing

- Lowercasing and text normalization
- URL and special character removal
- Stopword removal
- Tokenization
- Lemmatization using spaCy
- Cleaned dataset generation

Topic Modelling

- CountVectorizer for text vectorization
- Latent Dirichlet Allocation (LDA)
- Topic extraction and visualization
- Identification of dominant topics in news articles

Sentiment Analysis

- VADER sentiment analyzer
- Positive, Negative, and Neutral classification
- Sentiment score calculation
- Sentiment distribution visualization

Named Entity Recognition (NER)

- Entity extraction using spaCy
- Identification of:
  - PERSON
  - ORGANIZATION
  - LOCATION (GPE)
  - DATE
  - MONEY
  - PRODUCT

Interactive Dashboard

- Streamlit-based interface
- Dataset overview
- Topic insights
- Sentiment analytics
- Entity analysis
- Real-time visualization

---

Tech Stack

- Python
- Pandas
- NumPy
- NLTK
- spaCy
- Scikit-learn
- Plotly
- Streamlit
- Matplotlib

---

Project Structure

NLP_Text_Analytics_Pipeline/
│
├── preprocess.py
├── topic_model.py
├── sentiment.py
├── ner.py
├── app.py
├── cleaned_news.csv
├── bbc_news.csv
├── requirements.txt
└── README.md

---

Workflow

Step 1: Data Loading

The BBC News dataset is loaded and inspected using Pandas.

Step 2: Text Cleaning

The text is cleaned through:

- URL removal
- Stopword removal
- Punctuation removal
- Lemmatization

Step 3: Topic Modelling

LDA is used to identify hidden topics and categorize articles based on content themes.

Step 4: Sentiment Analysis

VADER calculates sentiment scores and classifies articles into positive, neutral, or negative categories.

Step 5: Named Entity Recognition

spaCy extracts important entities such as people, organizations, locations, and products.

Step 6: Dashboard Visualization

Results are displayed through an interactive Streamlit dashboard for easy analysis.

---

Installation

Clone the repository:

git clone <repository-url>
cd NLP_Text_Analytics_Pipeline

Install dependencies:

pip install -r requirements.txt

Download required NLP models:

python -m spacy download en_core_web_sm

Download NLTK resources:

import nltk

nltk.download('stopwords')
nltk.download('punkt')
nltk.download('vader_lexicon')

---

Running the Project

Run preprocessing:

python preprocess.py

Run topic modelling:

python topic_model.py

Run sentiment analysis:

python sentiment.py

Run named entity recognition:

python ner.py

Launch dashboard:

streamlit run app.py

---

Results

The project successfully:

- Cleans and preprocesses textual data.
- Extracts meaningful topics from news articles.
- Analyzes sentiment trends.
- Identifies important entities.
- Provides interactive visualizations for decision-making.

---

Future Enhancements

- BERT-based sentiment analysis
- Custom Named Entity Recognition models
- NewsAPI integration
- Real-time data streaming
- Semantic search functionality
- Automated alerts and notifications

---

Author

Mallela Srilekha

Data Science & NLP Project

Built as part of an NLP Text Analytics Pipeline project to demonstrate practical Natural Language Processing, Machine Learning, and Data Visualization skills.
