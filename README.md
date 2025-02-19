# MyMovie Notebook

## Overview

This Jupyter Notebook analyzes movie data from the dataset `mymoviedb.csv`. It utilizes data science libraries to explore, visualize, and derive insights from the dataset.

## Dependencies

The following Python libraries are required:

- `pandas` for data manipulation
- `seaborn` for visualization
- `matplotlib` for plotting
- `numpy` for numerical operations
- `warnings` to suppress warnings

## Dataset

The notebook loads a dataset named `mymoviedb.csv`. Ensure that this file is available in the same directory as the notebook.

## Features & Analysis

- Loads and preprocesses the movie dataset
- Performs exploratory data analysis (EDA)
- Generates visualizations to understand trends in movie data
- Applies statistical methods to derive insights

## Steps Taken

1. **Data Loading**: The dataset is loaded using pandas.
2. **Data Cleaning**:
   - Handled missing values (if any).
   - Checked for duplicates and removed them.
   - Converted data types where necessary (e.g., `Release_Date` to datetime, `Vote_Average`, `Vote_Count`, and `Popularity` to numeric) to enable proper analysis.
3. **Exploratory Data Analysis (EDA)**:
   - Visualized distribution of movie ratings.
   - Analyzed trends in movie release years.
   - Identified most popular genres.
4. **Statistical Insights**:
   - Calculated average ratings for different genres.
   - Determined factors influencing high-rated movies.
   - Examined correlations between different variables.

## Key Findings

- **English is the most common language for movie production, representing approximately 77% of all movies.**
- **A movie's popularity does not always correlate with a high rating.**
- **Over the years, movie production and popularity have increased significantly.**
- **Drama is the most common genre among produced movies.**
- **2021 recorded the highest number of movies produced.**
- **The movie with the highest popularity is *********Spider-Man: No Way Home********* (Action, Adventure, Science Fiction) with a popularity score of 5083.954.**
- **The movie with the lowest popularity is *********The United States vs. Billie Holiday********* (Music, Drama, History) with a popularity score of 13.354.**
- **Before filtering, the highest-rated movie was *********Kung Fu Master Huo Yuanjia********* (Action, Drama) with a rating of 10.0 but had only 1 vote, making it unreliable.**
- **After filtering out movies with fewer than 10% of the maximum votes, the highest-rated movie became *********The Godfather********* (Drama, Crime) with a rating of 8.7, which is a more reliable result.**
- **The most popular movie overall is *********Avengers: Endgame*********, while an unknown indie film had the lowest popularity.**
- **The movie with the highest number of votes is *********Inception********* (Action, Science Fiction, Adventure) with 31,077 votes and an average rating of 8.4.**
- **Applying a minimum voting threshold (10% of max voters) changed the highest rating from 10.0 to 8.7, indicating that movies with very few votes can skew results.**
- **There is a weak positive correlation (0.25) between Vote\_Count and Vote\_Average, meaning more votes slightly increase ratings, but not significantly.**
- **Popularity and Vote\_Average have almost no correlation (0.05), indicating that a popular movie is not necessarily highly rated.**
- **The correlation between Popularity and Vote\_Count is weak (0.14), meaning some popular movies may have fewer votes and vice versa.**
- **There is a slight negative correlation (-0.18) between Year and Vote\_Average, suggesting that newer movies tend to receive lower ratings than older ones.**
- **Year and Popularity show a weak positive correlation (0.13), meaning that recent movies tend to be more popular, but not strongly.**
- **As the number of voters increases, ratings usually range between 6 and 8, with fewer outliers.**
- **Newer movies tend to receive lower ratings compared to older ones.**
- **Most older movies fall within the 7-8 range, indicating they were generally rated positively.**
- **Starting from the 1970s and 1980s, there is a noticeable increase in the number of movies receiving very low ratings (<4).**

## Usage

1. Install the required dependencies:
   ```bash
   pip install pandas seaborn matplotlib numpy
   ```
2. Place `mymoviedb.csv` in the notebook directory.
3. Open the Jupyter Notebook and run the cells sequentially.

## Notes

- Ensure the dataset is clean and formatted correctly for better results.
- If any errors occur, check for missing values in the dataset and handle them accordingly.

