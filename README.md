# Song-Popularity-at-Spotify
What makes a song popular at Spotify, how does it affect stakeholders, and what are some interesting insights

We have songs from Spotify, which contains different kind of information about songs. In this exercise, we are trying to understand the factors driving popularity of the songs.

It is of interest to everyone who resonates with music. Often we like some songs which has high tempo and other sometimes songs with low tempo. So, if tempo alone is not a parameter, the question becomes crucial what does really require for a song to be famous?

The analytical approach will immensely help music composers/ artists in identifying right set of music attributes e.g., acoustics, instruments, liveliness, danceability, energy, valence etc.

# Objective

Understand the popularity of different songs with the help of insights and model. The objective is to create a map with music attributes and other information of songs with its popularity.

# Data

Source data contains 32853 rows and 23 columns.
Each row is presented for 1 song, however, there are few songs which are part of more than 1 playlist, gets repeated.
There are total 3 identifiers in data:
Track_id: Id of song
Artist_id: Id of artist
Album_id: Id of album
Playlist_id: Id of playlist song is part of

Popularity of songs is variable of interest and its value lies between 0 to 100, 0 being minimum and 100 maximum.
Data is collected in February 2020 as last released song in data is from January 2020.

# Predictive Modeling

Popularity is predicted as linear regression problem in RapidMiner tool. Below are steps of modeling:

1. Load data and check columns data types
2. Check summary statistics and histogram of each column
3. Perform missing value treatment
4. Create dummy variables using one-hot-encoding
5. Set role of Popularity as Label
6. Select useful attributes for the model
7. Build linear regression model using features and label
8. Apply model and assess the model performance

Model has the Root mean square error of 22.935

# Insights

# Impact 

Implication to artist:
The predictive model can work as a benchmark to assess the song or track before the release. The track can be readjusted with fine-tuning these attributes. In this way, the model will help the artists in gaining more hit songs.

Implication to listeners:
The usage of model will also help the people to get to listen more likeable songs. And have better music experience.

Implications to music business:
Platforms like Spotify, Amazon Music, Apple music, YouTube music etc. can benefit from increased user time on platform and can generate incremental revenue.

# Limitations

There are two main limitations of this work:
1. Additional information:
The model here relies on the data it has. There are many factors which are not included in this analysis and will be crucial, e.g. Time from last album, New Technology introduced, Song used in movie etc. These factors can change popularity a lot apart from factors used in this exercise.

2. Artist Bias:
Lot of time, a good song from lesser-known artist may not be that popular compared to average song from star artist.


# Tool
Understand data  ->Excel  
Data visualizations & insights -> Tableau
Data cleaning -> RapidMiner
Predictive Modeling -> RapidMiner
