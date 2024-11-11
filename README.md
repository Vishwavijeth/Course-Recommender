# Course-Recommender

This project implements a comprehensive AI-powered Course Recommender System using Streamlit, built as a capstone project for the IBM Machine Learning Professional Certificate. It features multiple recommendation algorithms, delivering course suggestions based on user preferences and ratings.

## Notebook overview

### 1. 01_EDA.ipynb - Exploratory Data Analysis
* Initial examination of the dataset.
* Analysis of course counts per topic to understand popularity.
* Ranking of users and courses by enrollments.
* Merge operation to associate course names with other attributes.

### 2. 02_FE.ipynb - Feature Engineering
* Merging course titles and descriptions to form a unified text field for feature extraction.
* Tokenization with NLTK, focusing on nouns and excluding stop words.
* Vocabulary creation using gensim, followed by Bag of Words (BoW) creation for each course.
* Computation of course similarity scores based on BoW, identifying similar courses.

### 3. 03_Content_RecSys.ipynb - Content-Based Recommendation Systems
* User Profile Model: Uses genre/feature weights to predict a user's rating for new courses based on their profile.
* Course Similarity Model: Recommends similar courses to users based on BoW similarities.
* User Profile Clustering: Reduces profile dimensions using PCA and clusters profiles with K-Means to recommend popular courses within clusters.

### 4. 04_Collaborative_RecSys.ipynb - Collaborative-Based Recommendation Systems
* Converts user-item ratings to sparse tables.
* Uses K-Nearest Neighbors (k-NN) for item- and user-based similarity predictions.


## Setup

### 1. Create Virtual env
```
python -m venv env
```
```
./env/Scripts/activate
```
### 2. Install requirements
```
pip install -r requirements.txt
```

### 3. Run
```
streamlit run recommender_app.py
```
