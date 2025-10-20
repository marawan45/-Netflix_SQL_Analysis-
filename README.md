# Netflix Data Analysis with SQL

This repository contains SQL queries used to analyze a dataset of Netflix titles and credits. The analysis aims to extract insights into content trends, popular genres, top-performing titles, and key contributors (actors and directors) on the Netflix platform.

# Table of Contents
## Project Overview

## Dataset

## Analysis Questions & Queries

## How to Use

## Contributing

## License

## Project Overview

This project focuses on performing a detailed SQL-based analysis of Netflix's content library. The SQL scripts provided answer various questions related to:

Distribution of movies vs. shows.

Release year trends.

Runtime analysis for both movies and shows.

Average IMDb and TMDB scores by various categories (type, country, age certification).

Identification of top actors and directors.

Genre popularity.

Titles with high ratings and popularity.

## Dataset

The analysis is based on two primary tables, presumably NetflixTitles and NetflixCredits.

NetflixTitles: Contains information about Netflix titles, including:

id

title

type (MOVIE or SHOW)

release_year

runtime

imdb_score

tmdb_score

age_certification

genres

production_countries

seasons (for shows)

NetflixCredits: Contains information about the cast and crew associated with each title, including:

id (linking to NetflixTitles)

name (of the person)

role (ACTOR, DIRECTOR, etc.)

character (if applicable)

(Note: The exact schema and column names are inferred from the provided SQL queries.)

## Analysis Questions & Queries
The SQL files (Netflix_SQL_Analysis.sql and Netflix_SQL_Analysis_2.sql) contain queries addressing the following questions:

General Content Overview
How many movies and shows are in the dataset?

How many movies/shows are released each year?

What were the total number of titles for each year?

Runtime Analysis
Which movie is the longest and which one is the shortest runtime?

Which show is the longest and which one is the shortest runtime?

What is the average runtime of each type (movie/show) by age certification?

Calculating the average runtime of movies and TV shows separately.

Rating and Popularity Analysis
What were the top 10 movies according to IMDb score?

What were the top 10 shows according to IMDb score?

What were the bottom 10 movies according to IMDb score?

What were the bottom 10 shows according to IMDb score?

What were the average IMDb and TMDB scores for shows and movies?

What were the average IMDb and TMDB scores for each production country?

What were the average IMDb and TMDB scores for each age certification for shows and movies?

How many movies in each IMDb Score?

Titles and Directors of movies with high IMDb scores (>7.5) and high TMDB popularity scores (>80).

Actors who have starred in the most highly rated movies or shows (IMDb score > 8.0 and TMDB score > 80).

Genre and Certification Analysis
What were the 5 most common age certifications for movies?

Which genres had the most movies?

Which genres had the most shows?

Cast and Crew Analysis
Who were the top 20 actors that appeared the most in movies/shows?

Who were the top 20 directors that directed the most movies/shows?

Finding the titles and directors of movies released on or after 2010.

Which actors/actresses played the same character in multiple movies or TV shows?

Show Specific Analysis
Analyze the seasons of Netflix Shows/Series.

Which shows on Netflix have the most seasons?

Time-based Analysis
Count of movies and shows in each decade.

## How to Use
To use these SQL queries:

Database Setup: Ensure you have a SQL database (e.g., SQL Server, MySQL, PostgreSQL) set up.

Load Data: Import your Netflix titles and credits data into two tables named NetflixTitles and NetflixCredits respectively, matching the column names inferred from the queries.

Execute Queries: Open the .sql files in your preferred SQL client or IDE and execute the queries. You can run them individually or in batches to get the desired insights.
