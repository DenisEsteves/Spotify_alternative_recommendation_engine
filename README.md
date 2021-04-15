# Spotify alternative recommendation engine 🎵🥁🎵

## Problem

Spotify is the world’s most popular audio streaming subscription service. Their more than 320million users can listen to more than 60 million tracks.Due to that vast different options, a recommendation engine is needed.

However Spotify is trying to recommend songs and singers according to their business and not only to the user's preferences, which sometimes lead to not right recommendations.

My proposal is to create a recommendation engine that takes into account the song characteristics only. Those features that unconscientely the user likes.

## Methodology

Using the dataset taken from [Kaggle](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks) and machine learning, I created an alternative Spotify recommendation engine that takes into account purely the characteristics of the song to do new recommendations. This characteristics are the following:
                              - Valence
                              - Year
                              - Acousticness
                              - Danceability
                              - Duration 
                              - Energy
                              - Explicit
                              - Instrumentalness
                              - Liveness
                              - Loudness
                              - Mode
                              - Popularity
                              - Speechiness
                              - Tempo

I used the K-means prediction method. This is an unsupervised learning technique to classify unlabeled data by grouping them by features. The number of optimal clusters was given by the use of the Elbow method. The result was 10. Therefore, I created 10 clusters of songs with similar characteristics. 

Doing to the user choose in a small questionnaire between a couple of songs (If they are unknown songs, the user can play a 30 secs sample or see the song cover), the user preferences can be clustered. Thus, songs with similar characteristics can be recommended to the him. 
