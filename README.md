# Music Listening Habits and Productivity Analysis
## **Project Overview**
This project explores the relationship between music listening habits and productivity during study or work sessions. By analyzing personal data on music preferences, task performance, and working hours, the project seeks to uncover patterns and provide actionable insights for optimizing productivity through personalized music recommendations. The project combines data-driven analysis techniques, including exploratory data analysis (EDA), machine learning models, and visualization, to generate meaningful findings. 

## **Motivation**
Music is a powerful tool for enhancing focus and productivity. This project aims to analyze how specific music attributes such as genre, tempo, and loudness influence productivity during various task types. By understanding these relationships, we can create personalized music strategies for optimal work or study performance.

## **Dataset Description**

### **Music Listening Data**
- **Source**: Spotify API and AcousticBrainz API (where Spotify's API was limited or deprecated)
- **Fields**:
  - `Track Name`: Title of the song.
  - `Artist`: Artist of the song.
  - `Genre`: Genre classification of the song (e.g., Pop, Classical, Jazz).
  - `Tempo`: Beats per minute (BPM) of the song.
  - `Loudness`: Volume of the track in decibels.
  - `Listening Timestamp`: The time when the song was played.
 
### **Productivity Data**
- **Source**: Manually logged or extracted from a time-tracking tool.
- **Fields**:
  - `Task Type`: The type of the task (e.g., Writing, Coding, Reading).
  - `Duration`: Total hours worked in the session.
  - `Task Completion Time`: Duration required to complete the task.

## **Project Objectives**
1. Analyze the correlatation between music features and productivity during different task types.
2. Build a predictive model to recommend optimal music genres for specific task types.
3. Provide visualizations and actionable insights for personalized productivity strategies.

## **Project Plan**

### **Data Collection**
- **Music Data**:
  - Retrieved using Spotify API for track metadata and listening history.
  - Supplemented with audio features such as tempo and loudness from AcousticBrainz API.
- **Productivity Data**:
  - Manually recorded task types, durations, and timestamps.
  - Synced with music listening data for temporal alignment.

### **Data Preprocessing**
- **Steps**:
  - Cleaned datasets for consistency and removed duplicates.
  - Merged music and productivity data based on timestamps.
  - Missing values in Tempo and Loudness have been replaced with genre-specific medians where available, and the overall median as a fallback.
  - Feature engineering:
    - Average tempo, loudness, and genre distribution per session.
   

### **Exploratory Data Analysis (EDA)**
- **Techniques Used**:
  - Correlation analysis between music attributes and productivity.
  - Visualization of:
    - Music attributes over time.
    - Productivity trends across task types and working hours.
  - Tools: Scatterplots, heatmaps, and time-series graphs.
 
### **Modeling**
- **Techniques**:
  - **Clustering**: Identify groups of sessions with similar music attributes and productivity levels.
  - **Regression**: Predict productivity scores using features like tempo, loudness, and task type.
  - **Time-Series Analysis**: Forecast productivity based on music listening trends.
- **Goal**: Create a model that suggests music attributes for optimal productivity.

### **Findings**

### **Insights and Recommendations**
   - Provide a summary of findings:
     - Best genres or tempos for productivity.
     - Ideal working hours for specific music types.
   - Develop actionable recommendations:
     - Suggest personalized playlists for study/work.

### **Limitations and Future Work**
- **Limitations**:
  - Incomplete or missing data for some tracks due to API restrictions.
  - Manual logging of productivity data, leading to potential inconsistencies.
- **Future Plans**:
  - Automate productivity tracking.
  - Explore advanced machine learning techniques for more accurate predictions.
  - Create a recommendation system for generating personalized playlists.
 
## **Visualization and Reporting**
- **Deliverables**:
  - Visualizes trends, correlations, and recommendations.
  - Suggests music genres and tempos for productivity improvement.

## **Repository Structure**
