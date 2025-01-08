# Music Listening Habits and Productivity Analysis
## **Project Overview**
This project explores the relationship between music listening habits and productivity during study or work sessions. By analyzing personal data on music preferences, task performance, and working hours, the project aims to uncover patterns and provide actionable insights for optimizing productivity through personalized music recommendations.

## **Dataset Description**

### **Music Listening Data**
- **Source**: Spotify API
- **Fields**:
  - `Track Name`: Title of the song.
  - `Artist`: Artist of the song.
  - `Genre`: Genre classification of the song (e.g., Pop, Classical, Jazz).
  - `Tempo`: Beats per minute (BPM) of the song.
  - `Energy`: A measure of the song’s intensity and activity (range: 0-1).
  - `Loudness`: Volume of the track in decibels.
  - `Listening Timestamp`: The time when the song was played.
 
### **Productivity Data**
- **Source**: Manually logged or extracted from a time-tracking tool.
- **Fields**:
  - `Task Type`: The type of the task (e.g., Writing, Coding, Reading).
  - `Duration`: Total hours worked in the session.
  - `Task Completion Time`: Duration required to complete the task.

## **Project Objectives**
1. Analyze the relationship between music attributes and productivity.
2. Build a predictive model to recommend optimal music genres and tempos for specific task types.
3. Provide visualizations and actionable insights for personalized productivity strategies.

## **Project Plan**

### **Data Collection**
   - Retrieve music listening data using the Spotify API.
   - Track productivity scores, task types, and working hours manually or via apps.
   - Align timestamps to link music listening sessions with productivity data.

### **Data Preprocessing**
   - Clean and merge datasets
   - Feature engineering:
     - Derive metrics like average tempo, energy levels, and genre distribution per session.

### **Exploratory Data Analysis (EDA)**
   - Analyze correlations between:
     - Music attributes (tempo, energy, genre) and productivity.
     - Working hours and productivity scores.
   - Visualize patterns using scatterplots, heatmaps, and time-series graphs.

### **Modeling**
   - **Clustering**:
     - Group sessions based on music attributes and productivity to identify patterns.
   - **Regression**:
     - Predict productivity scores using features like tempo, energy, and task type.
   - **Time-Series Analysis**:
     - Model productivity trends over time and forecast optimal music attributes for future tasks.
    
### **Insights and Recommendations**
   - Provide a summary of findings:
     - Best genres or tempos for productivity.
     - Ideal working hours for specific music types.
   - Develop actionable recommendations:
     - Suggest personalized playlists for study/work.
    
### **Visualization and Reporting**
   - Build an interactive dashboard:
     - Display trends and insights.
     - Provide real-time productivity recommendations.
