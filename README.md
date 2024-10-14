# Spotify Song Recommendation System
## Project Overview
This project implements a **personalized song recommendation system** using the **Upper Confidence Bound (UCB) algorithm**. The recommendation process is enhanced by incorporating user feedback, which is influenced by the **time of day**. The aim is to provide users with a dynamic and relevant playlist by learning their preferences and adjusting song recommendations based on their listening habits throughout the day.

## Table of Contents
+ Project Motivation
+ Dataset
+ Algorithm and Approach
+ Libraries Used
+ Results and Performance
+ Future Improvements
+ Contributing

## Project Motivation
The objective of this project is to explore how machine learning algorithms, specifically the **Upper Confidence Bound (UCB)**, can be applied in recommendation systems. By leveraging feedback based on the time of day, this project seeks to offer users music that best suits their mood and preferences at different times, enhancing the user experience on platforms like Spotify.

## Dataset
The dataset used in this project is based on Spotify's song data, retrieved using the **Spotify Web API**. Each song is described by features such as its genre, popularity, artist, and tempo. The user interaction data includes:

+ Song history (songs listened to by the user)
+ Time of day when each song was played
+ User feedback (positive/negative based on whether they liked the recommendation)

## Algorithm and Approach
### Upper Confidence Bound (UCB)
The UCB algorithm is a reinforcement learning technique that balances the trade-off between exploration (trying new songs) and exploitation (recommending songs that are likely to be enjoyed based on past feedback). The formula used to calculate UCB is:

### Feedback Based on Time of Day
To make the recommendations more personalized, user feedback is influenced by the time of day. The system assumes that users may prefer different types of songs depending on the time. For example:

+ Morning: Calmer, upbeat tracks
+ Afternoon: Energizing or focus-oriented songs
+ Evening: Relaxing or mood-setting music

By integrating this time-based feedback, the recommendation system adapts its suggestions throughout the day.

## Libraries Used
This project relies on the following libraries:

+ datetime: To handle time-based data and adjust recommendations based on the time of day.
+ math: For mathematical operations, including the calculation of the UCB algorithm.
+ matplotlib.pyplot: For plotting graphs and visualizing results.
+ spotipy: To interact with the Spotify API and retrieve song data.
+ spotipy.oauth2: To authenticate and authorize API requests using OAuth 2.0.

## Results and Performance
The system successfully implements dynamic song recommendations. By utilizing the UCB algorithm, the system strikes a balance between exploring new songs and exploiting user-favored songs. Additionally, the feedback mechanism based on the time of day has shown promising results in improving user satisfaction with recommendations.

## Key Metrics:
+ User engagement: Increased due to personalized recommendations.
+ Adaptability: The system adjusts song recommendations based on the user's time of day and mood.

## Future Improvements
+ Enhanced feedback mechanisms: Collect more detailed user feedback, such as song skips or likes/dislikes, to improve recommendations.
+ Incorporate additional features: Use more song metadata like genre, tempo, and mood classification to enhance personalization.
+ Multi-user recommendations: Expand the system to recommend songs for groups of users with shared preferences.
+ Real-time adaptability: Make the system responsive to changes in user behavior in real-time.

## Contributing
Feel free to fork the repository and make contributions. Pull requests are welcome! Please ensure that you adhere to the project's coding standards and guidelines.
