## Anime popularity analysis

This project analyzes anime ratings using the Anime Recommendation Database 2020, focusing on data cleaning, preprocessing, merging, and exploratory analysis. The analysis is implemented in a Jupyter Notebook (Anime.ipynb).

The goal is to clean the raw data, prepare a high-quality dataset, and explore patterns such as top-rated anime, genres, and rating distributions.

##  Data Set

The project uses two datasets:
anime.csv
rating.csv.zip (contains rating.csv)

Anime dataset columns
anime_id
name
genre
type
episodes
rating
members

Rating dataset columns
user_id
anime_id
rating (−1 means watched but not rated)

##  Workflow Overview
1. Import libraries

Uses the following libraries:
pandas
numpy
zipfile

2. Load datasets

rating.csv is extracted and loaded from a ZIP file
anime.csv is loaded directly

3. Data CleaningAnime table cleaning
Strip column names
Convert anime_id, episodes, members to numeric
Fill missing:
-name → "Unknown"
-rating → median rating
-genre → "Unknown"
Remove or fix irregular values

Rating table cleaning
Strip column names
Convert user_id, anime_id, rating to numeric
Remove rows where rating = -1
Drop rows with missing values
Remove duplicated (user_id, anime_id) pairs, keeping the latest rating

4. Merge datasets
The rating and anime tables are merged using anime_id:
df = pd.merge(rating, anime, on="anime_id")

5. Exploratory Data Analysis (EDA)
Includes visual and statistical exploration such as:
Rating distribution
Most rated anime
Highest average ratings
Genre frequency
Average rating by anime type
User rating patterns

##  Visualisation

The notebook may include charts such as:
Histogram of user ratings
Bar charts for genre counts
Top anime by rating or popularity
Type distribution (TV, OVA, Movie, etc.)
Correlation matrix
All visualizations appear directly inside the notebook.

##  Example Insight

(Modify based on your results)
Users tend to give mid-range ratings
Certain genres like Action or Drama appear most frequently
Some anime with the most members do not have the highest ratings
TV-type anime dominate the dataset
