# Spotify Songs Analysis Project

This project analyzes data from the "Top Spotify Songs 2023" dataset, which includes information about songs, artists, and their streaming statistics.

## Dataset Information

The dataset consists of the following columns:

- **track_name:** Name of the song
- **artist(s)_name:** Name of the artist(s) of the song
- **artist_count:** Number of artists contributing to the song
- **released_year:** Year when the song was released
- **released_month:** Month when the song was released
- **released_day:** Day of the month when the song was released
- **in_spotify_playlists:** Number of Spotify playlists the song is included in
- **in_spotify_charts:** Presence and rank of the song on Spotify charts
- **streams:** Total number of streams on Spotify
- **in_apple_playlists:** Number of Apple Music playlists the song is included in
- **in_apple_charts:** Presence and rank of the song on Apple Music charts
- **in_deezer_playlists:** Number of Deezer playlists the song is included in
- **in_deezer_charts:** Presence and rank of the song on Deezer charts
- **in_shazam_charts:** Presence and rank of the song on Shazam charts
- **bpm:** Beats per minute, a measure of song tempo
- **key:** Key of the song
- **mode:** Mode of the song (major or minor)
- **danceability_%:** Percentage indicating how suitable the song is for dancing
- **valence_%:** Positivity of the song's musical content
- **energy_%:** Perceived energy level of the song
- **acousticness_%:** Amount of acoustic sound in the song
- **instrumentalness_%:** Amount of instrumental content in the song
- **liveness_%:** Presence of live performance elements
- **speechiness_%:** Amount of spoken words in the song

## Data Cleaning and Preprocessing

In the course of preparing this project, the dataset underwent several cleaning and preprocessing steps to ensure its quality and consistency. The following tasks were performed in an IPython Notebook (ipynb) prior to importing the dataset into the SQL database:

1. **Handling Missing Values:** Missing values in the dataset were identified and handled by dropping rows with missing values and converting numeric columns to the appropriate data types.

2. **Renaming Columns:** Column names were modified for better clarity, making the dataset more user-friendly.

3. **Standardizing Artist Names:** Artist names were standardized to ensure consistency, including replacing commas (',') with 'and' and removing non-English characters.

4. **Managing Long Names:** For cases where track or artist names were excessively long, they were truncated to maintain data integrity.
   
## SQL QUERIES

1. **Retrieve Song Details with Most Features:** Retrieve the names of all the songs in the dataset along with their corresponding artist names, release years, and danceability percentages.

2. **Count of Unique Artists in Spotify Charts:** Find the number of unique artists whose songs appear in the Spotify charts.

3. **Top Artists by Stream Count:** List the top 5 artists with the highest total streams across all their songs in the dataset.

4. **High Energy and Danceability:** Identify songs with both an energy percentage above 80% and a danceability percentage above 75%.

5. **Most Popular Song in Deezer Playlists:** Find the song with the highest number of inclusions in Deezer playlists.

6. **Average Danceability by Release Year and Month:** Calculate the average danceability percentage for songs released in each year and month. Provide the results in a table with columns for the year, month, and the average danceability.

7. **Spotify vs. Apple Music Popularity with Presence Score:** Determine which songs are more popular on Spotify compared to Apple Music. Create a metric called "Presence Score" that combines the presence in both Spotify and Apple Music charts. List songs with a Presence Score above a certain threshold (e.g., 100) along with their artists and Presence Scores.

8. **Rank Artists by Their Total Streams Across All Tracks:** Rank artists by the total number of streams across all their tracks and identify the top 5 and bottom 5 artists.

## Project Purpose

The primary purpose of this project is to deepen my understanding of SQL, hone my data analysis skills, and explore various SQL queries and techniques. This project is a practice project, and I plan to modify it in the course of time as I discover new topics and optimization techniques. Furthermore, I have plans to collect datasets that require extensive data cleaning and preprocessing in the future. These datasets will serve as the foundation for new projects, which I intend to develop either in SQL or Python.

## Acknowledgments

- **Dataset source:** [Top Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023)
