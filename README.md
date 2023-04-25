# music_recommendation

# How does it work?
Basically, it asks for the user to select their favorite tracks from Spotify, then it compares each of them - one by one - with every track in the recommender dataset. In order to do this it gets the tracks' audio features provided by the Spotify API and computes the euclidean distance between the inputted tracks and the dataset tracks to generate a similarity index. The recommended tracks are the ones from the dataset with the highest similarity index compared to each of the inputted tracks (closest to 1.0).

# The distance
The general idea is to compare the difference between all the features of the inputted tracks against the features of each of the tracks in the dataset. To do this, we use euclidean distance.
