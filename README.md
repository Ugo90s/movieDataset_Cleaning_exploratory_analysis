# MovieDataset_Cleaning_exploratory_analysis
Data cleaning and analysis on latest IMDb movie dataset.
Python Version 3.10.9 IDE: Jupyter Notebook

In this Python data analysis project, the latest imdb movie dataset is explored to derive insights in various aspect of movie production. Key python libraries such as Pandas, Matplotlib and Seaborn were used to achieve effective data manipulation and visualization.

## DataSet Overview

This dataset consist of 400 data entries with each record representing a movie title and 8 corresponding columns with information such as IMDb Rating (aka user reviews), Year, Certificates (aka film rating), Genre, Director, Star Cast, MetaScore, Duration (minutes)

## Data Cleaning

Initial steps were taken to clean data and ensure data integrity such as checking dataset shape to confirm accurate number of rows and column, checking for null values, printing out descriptive statistics to ensure no anomalies in numerical entries and check for any outliers

## Duplicates

Duplicate entries were checked and deleted to avoid redundant data

## EDA - Exploratory Data Analysis

This was helpful to discover patterns and derive insights from the dataset which includes learning the average movie duration for all movies in the dataset, identifying lenghty movies, discovering number of movies produced each year, finding top movie directors (by its movie rating), a scatterplot to showcase movie rating over the years

<img src="https://github.com/Ugo90s/movieDataset_Cleaning_exploratory_analysis/blob/main/movie_rating_byYear.png" width=60% height=50%>

<img src="https://github.com/Ugo90s/movieDataset_Cleaning_exploratory_analysis/blob/main/top_movieGenre.png" width=60% height=50%>


## Top Movie Rating and classifying movies as "Excellent", Good, or Average

Identified popular movies based on its movie rating, also set up an additional column to classify movies as Excellent, good or average based on its rating

## Popular Genre (based on Movie rating)

Showcased top movie Genres and its corresponding movie title

## Tools and List of Functions used in this Movie Dataset Analysis Project;

1. **Pandas Functions:**
   - `pd.read_csv()` - this reads the dataset from .csv file
   - `isnull().sum()` - outputs a count of missing values for each field
   - `duplcated().any()` - checks for duplicate data across the dataset
   - `drop_duplicates()` - deletes all duplicate value
   - `describe()` - provides statistical information about the dataset
    
2. **Matplotlib Functions:**
   - `plt.title()`- adds a title to the plot.
   - `plt.xticks(rotation= )`- formats the x-axis
   - `plt.show()`- displays the plot.

3. **Seaborn Functions:**
   - `barplot(x, y, data)`- creates bar graph visual.
   - `countplot(x, data)`- counts x values and displays plot
   - `scatterplot(x, y, data)`- showcases relationship between two variables in a scatterplot.
  
## Limitations/Feedback

1. Dataset had alot of redundant/duplicate data which overall questions the integrity of the data source
2. Additional columns such as "Revenues" would have been helpful for further analysis such as finding any correlations between "Ratings" and "Revenue", checking if there is any consistent pattern or preferrence for a specific movie genre over time based on Revenues
3. Dataset seems to be quite inconsistent with the number of movies produced over the years, e.g some years showcased just one movie produced, and information doesn't align with imdb website
