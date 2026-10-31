# Personality Prediction from Social Media

Predicts a user's MBTI personality type (one of 16 types) from social media text using NLP and machine learning.

Project Link: https://personalitypredictionfromsocialmedia.netlify.app/

## Technologies Used
- Python, Pandas, NLTK
- Sentence-Transformers (BERT embeddings), XGBoost, SMOTE
- Django, SQL (SQLite), HTML, CSS
- Streamlit

## Project Structure
- cleaning.py: cleans and preprocesses the text data
- training.py: creates BERT embeddings and trains the XGBoost model
- streamlit_app.py: Streamlit app for live prediction
- django_app/: Django web app with an HTML/CSS form; predictions are saved in an SQL database
- model/: saved model and label encoder
- data/: cleaned dataset

## How to Run
1. pip install -r requirements.txt
2. Streamlit app: streamlit run streamlit_app.py
3. Django app: cd django_app, then python manage.py makemigrations predictor, python manage.py migrate, python manage.py runserver

## My Role
- Collected and cleaned social media text data using Pandas.
- Connected Python with Django, so the trained model runs behind a web interface.
- Built the HTML/CSS form for user input and used SQL (SQLite) to store predictions.
