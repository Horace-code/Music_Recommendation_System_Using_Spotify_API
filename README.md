# Music_Recommendation_System_Using_Spotify_API
## Overview
This project utilizes the Spotify API, a powerful tool that allows developers to access Spotify's extensive music catalog and collect music-related data. By leveraging Spotify's API, we create a Music Recommendation System that provides personalized music suggestions to users.
The recommendation system operates through sophisticated algorithms that analyze users' musical interactions, such as listening history, liked tracks, and skipped songs. These algorithms construct user profiles and generate music recommendations based on these profiles. The system combines content-based filtering, collaborative filtering, and hybrid approaches to enhance the accuracy and relevance of recommendations.

## Features
Authentication: The system uses the Spotify API for authentication, requiring developers to obtain client credentials to access Spotify's data.
Data Collection: Real-time music data is collected from Spotify, including track names, artists, albums, release dates, popularity, and audio features.
Content-Based Filtering: The system generates music recommendations based on audio features such as danceability, energy, loudness, and valence.
Weighted Popularity: Recommendations are weighted based on the popularity of the songs and their release dates, ensuring a balance between popularity and recency.
Hybrid Recommendations: The system combines content-based recommendations with weighted popularity scores, providing personalized and relevant suggestions to users.

## How to Use
To use this Music Recommendation System, follow these steps:

### Set Up Spotify Developer Account:

Create a Spotify developer account and obtain client credentials (Client ID and Client Secret) to authenticate the application.
Create a new app in the Spotify Developer Dashboard and obtain the credentials.
Install Dependencies:

Install required Python libraries using the following command:
Copy code
pip install spotipy pandas scikit-learn
Run the Code:

Update the CLIENT_ID and CLIENT_SECRET variables in the code with your obtained credentials.
Run the Python script to collect music data from a specified Spotify playlist and generate recommendations.
Explore Recommendations:

Input a song name to get personalized recommendations based on its audio features and popularity.
Example Usage
python
Copy code
input_song_name = "I'm Good (Blue)"
recommendations = hybrid_recommendations(input_song_name, num_recommendations=5)
print(f"Hybrid recommended songs for '{input_song_name}':")
print(recommendations)
