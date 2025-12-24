## Anime popularity Analysis & Recommender System

## Project Overview
This project analyzes anime popularity data and builds a simple recommender system to suggest similar anime based on user preferences and content similarity. The goal is to demonstrate an end-to-end data workflow: data cleaning, exploratory data analysis (EDA), feature engineering, and recommendation logic.

The project is designed as a portfolio project for data analytics / data science roles and focuses on explainability and insights rather than complex deep learning models.

## Problem Statement
With thousands anime titles available, users often struggle to discover shows that match their interests. This project aims to:
- Understand what factors influence anime popularity
- Explore relationship between ratings, genres, and user engagement
- Build a recommender system that suggests similar anime titles

##  Data Set
- Source: Public anime dataset (e.g. MyAnimeList / Kaggle)
- Content:
Anime title
Genres
User ratings
Popularity / number of members
- Size: Thousands of anime records

## Tools & Technologies
- Python
- pandas, Numpy
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook

##  Data Preparation
Key data processing steps include:
- Handling missing and inconsistent values
- Cleaning and standardising genre information
- Converting categorical text features into numerical representations
- Normalising popularity and rating features

## Exploratory Data Analysis (EDA)
The EDA focuses on understanding popularity patterns and user preferences:
- Distribution of anime ratings and popularity
- Most common genres and genre combinations
- Relationship between rating score and popularity
- Identification of highly rated but less popular anime
Key observations:
- Certain genres consistently achieve higher average ratings
- Popularity does not always correlate strongly with rating score
- Niche genres often have high ratings but smaller audiences

## Recommender System Approach
A content-based recommender system is implemented:
- Anime titles are represented using genre and rating features
- Similarity between anime is computed using cosine similarity
- Given an input anime, the system returns the top‑N most similar titles
This approach is suitable when user‑level interaction data is limited.

## Results & Example Output
- The recommender successfully suggests anime with similar genres and rating profiles
- Recommendations are intuitive and interpretable
- Results demonstrate how simple similarity‑based methods can be effective for recommendation tasks

## Limitations & Future Improvements
- Does not incorporate user‑specific behaviour (collaborative filtering)
- Genre labels are treated equally without weighting
Future work could include:
- User‑item interaction data
- Matrix factorisation or neural recommenders

## Conclusion
This project demonstrates practical skills in:
- Data cleaning and exploratory analysis
- Feature engineering for real‑world datasets
- Building an interpretable recommender system
It showcases the ability to translate raw data into insights and functional data products, relevant for data analyst and data science roles.
