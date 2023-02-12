# Spotify EDA and Linear Regression
As a guitar player and an avid music fan, I thought it would be interesting to explore what the components of top hit songs are and gain new insights related to the making of top music hits. The purpose of this project is to perform exploratory data analysis on Spotify music data, and later try to predict popularity based on the dataset's attributes.

## The Dataset (link to Kaggle dataset is [here](https://www.kaggle.com/datasets/paradisejoy/top-hits-spotify-from-20002019))

The dataset comes from Kaggle user Mark Koverha and can be found in the link above, and, in the words of the author, it consists of the following columns:

1. ***Artist:*** Name of the Artist.

2. ***Song:*** Name of the Track.

3. ***Duration_ms:*** Duration of the track in milliseconds.

4. ***Explicit:*** The lyrics or content of a song or a music video contain one or more of the criteria which could be considered offensive or unsuitable for children.

5. ***Year:*** Release Year of the track.

6. ***Popularity:*** The higher the value the more popular the song is.

7. ***Danceability:*** Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

8. ***Energy:*** Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity.

9. ***Key:*** The key the track is in. Integers map to pitches using standard Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1.

10. ***Loudness:*** The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.

11. ***Mode:*** Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.

12. ***Speechiness:*** Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.

13. ***Acousticness:*** A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.

14. ***Instrumentalness:*** Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.

15. ***Liveness:*** Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.

16. ***Valence:*** A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

17. ***Tempo:*** The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.

18. ***Genre:*** Genre of the track.

## EDA Conclusions 
- Top Artists by number of top hits: Rihanna, Drake, Eminem, Calvin Harris, Britney Spears, David Guetta, Chris Brown, Katy Perry, Beyoncé, and Taylor Swift.

- Top Artists with a minimum of 5 Top Hits and Average Song Popularity: Bruno Mars, Marshmello, Arctic Monkeys, Red Hot Chili Peppers, Linkin Park, Coldplay, Fall Out Boy, Sam Smith, Lady Gaga, Ed Sheeran.

- Song duration has been steadily decreasing from the year 2000 to 2019.

- The most frequent genres in top hits: Pop, Hip Hop, R&B, Dance/Electronic, and Rock.

- The 10 most popular songs in the dataset in order were: Sweater Weather by The Neighbourhood, Another Love by Tom Odell, Without Me by Eminem, The Real Slim Shady by Eminem, Lovely by Billie Eilish with Khalid, Wait a Minute! by WILLOW, Circles by Post Malone, The Nights by Avicii, Perfect by Ed Sheeran, Locked Out of Heaven by Bruno Mars.

## Linear Regression
I decided to also practice some of my machine learning skills and try to build a model to predict song popularity based on the attributes in the dataset using linear regression. 
