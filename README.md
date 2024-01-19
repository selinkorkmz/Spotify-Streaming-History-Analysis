# Spotify-Streaming-History-Analysis

# Spotify Listening History Analysis Project

## Overview

This project explores my own Spotify listening history to gain insights into my music preferences, habits, and how they evolve over time. By delving into different time periods, such as weekdays, weekends, mornings, evenings, and seasonal changes, the analysis aims to uncover patterns and trends in my music consumption.

## Motivation

I initiated this project to go beyond Spotify's yearly summaries and gain a more detailed understanding of my music habits. The motivation behind this exploration was to uncover insights that traditional summaries might not capture, such as how my preferences vary based on specific times of the day, days of the week, and even seasonal changes.

## Data Source

-The primary data source for this project is my Spotify listening history (StreamingHistory-.json) that I requested from Spotify. 
-The data for song's details are collected through Spotify's API, allowing for a detailed examination of each song for their artists, genres, and more.

## Data Analysis

### Techniques Used

- **Exploratory Data Analysis (EDA):** Initial exploration of the dataset to understand its structure and key features.
- **Time-based Analysis:** Grouping data based on different timeframes, such as weekdays, weekends, mornings, night, summer and winter.
- **Genre and Artist Analysis:** Exploring changes in top genres and artists different groups of over time.
- **Listening Durations Analysis:** Exploring changes in listening durations over different groups of time.
  
### Analysing Steps
**Data Collection and Preprocessing:**

- Gathered Spotify listening history, including track details and timestamps.
- Extracted relevant features like 'dayOfWeek,' 'dayOfYear,' and 'timeOfDay.'
- Converted timestamps to datetime objects for ease of analysis.
- Filtered data to focus on specific time periods (e.g., summer, winter).

**Genre Analysis:**

- Utilized Spotify API for artist and genre information.
- Mapped artists to their associated genres using API responses (functions like `searchArtist()` and `getToken()` in the code).
- Explored changes in genre preferences over different times of the day or months.
- Identified and visualized top genres during specific time frames.

**Top Artist Analysis:**

- Leveraged Spotify API to search for top artists based on their names.
- Stored relevant information about top artists, including genres and popularity.

**Time-of-Day Analysis:**

- Grouped data based on the 'timeOfDay' feature (morning, night).
- Calculated average listening time for each time of day.
- Visualized distribution of listening time during mornings and nights.

**Day-of-Week Analysis:**

- Grouped data based on the 'dayOfWeek' feature.
- Explored and visualized differences in listening habits and times between weekdays and weekends.

**Seasonal Analysis (Summer-Winter):**

- Created subsets of data for summer and winter months.
- Investigated changes in listening behavior, genres, and top artists between seasons.
- Visualized and compared trends during summer and winter periods.

  

### Findings

- Insights into how my listening durations and music preferences change at different times.
- Understanding the impact of different timeframes on my favorite artists.
- Recognizing variations in music consumption between different times and possible causes of it.
- An example from my Hypotheses: During the academic months (10, 11, 12), there is a discernible variance in my music listening patterns between morning and night. In the morning hours (9-11), particularly while commuting to school, witness a higher frequency of music consumption compared to the night hours.
  
**You can find more detailed information from my project report - presentation.**
  
## Limitations and Future Work
### Genre Information from Artist Associations

The analysis heavily relied on associating genres with artists. However, this approach might not fully capture the diversity within an artist's discography. Further improvements could involve obtaining genre information directly from Spotify or using more sophisticated methods to categorize music genres.

### Lack of External Factors

The analysis primarily focused on internal factors like time of day and season. External factors such as mood, external events, or even global occurrences could significantly impact music preferences. Future iterations of this project could incorporate additional external data sources to provide a more holistic view of the influences on music consumption.

### Future Work
The project has potential for further enhancements and future developments:

- **Machine Learning Models for Prediction:** Applying machine learning models to predict musical preferences based on various criteria.
- **Active Visualization:** Creating interactive dashboards to make Spotify listening history insights more engaging and user-friendly.


## How to Use

To replicate or contribute to this project, follow these steps:

1. Clone the repository: `git clone https://github.com/selinkorkmz/spotify-analysis.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Execute the analysis scripts: `python analyze_spotify.py`

Feel free to explore the Jupyter notebooks, data visualizations, and contribute to the project.

## Prerequisites

Before running the analysis, make sure you have the following dependencies installed:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
  
## Contributors
Ayse Selin Korkmaz

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
