# YouTube Trending Videos Analysis

## Introduction
This project analyzes YouTube trending videos using the YouTube Data API. The goal is to identify patterns in trending content, such as the best time to post, ideal video length, and factors that contribute to high engagement (views, likes, and comments). By analyzing video metadata, we provide insights for content creators and marketers to optimize their strategies.

## Problem Statement
Understanding what makes a video trend on YouTube is crucial for content creators. However, YouTube does not provide direct insights into the best posting times, video duration, or engagement factors. This project aims to:
- Identify the best time to post videos in India.
- Determine the ideal video length for higher engagement.
- Analyze trends in views, likes, and comments across different categories.

## Project Workflow
1. **Data Collection:**
   - Fetched trending video data using the YouTube Data API.
   - Extracted key metrics such as title, description, publish time, views, likes, and comments.
   
2. **Data Cleaning & Processing:**
   - Converted timestamps from UTC to IST (Indian Standard Time).
   - Extracted the hour of publication to analyze the best posting times.
   - Handled missing values and removed duplicate entries.
   
3. **Data Analysis & Insights:**
   - Identified peak hours for posting trending videos.
   - Analyzed video duration vs. engagement levels.
   - Created visualizations to showcase patterns in trending content.

## Database
- The dataset was processed using **pandas DataFrames**.
- No external database was used, but the project can be scaled using MySQL or PostgreSQL.

## Challenges Faced
- **API Limits:** The YouTube Data API restricts the number of requests per day, requiring optimized data fetching.
- **Time Zone Adjustments:** YouTube timestamps are in UTC, so they had to be converted to IST for accurate analysis.
- **Data Cleaning:** Some videos had missing descriptions or comments, which required appropriate handling.

## Key Findings
- **Best Time to Post:** Videos posted between **6 PM - 9 PM IST** tend to get the highest engagement.
- **Ideal Video Length:** Videos ranging from **8 to 12 minutes** perform the best in terms of views and likes.
- **Category Trends:** Entertainment and music videos dominate the trending section.

## Tech Stack
- **Python** (for data extraction and analysis)
- **YouTube Data API** (for collecting video data)
- **pandas** (for data processing)
- **Matplotlib & Seaborn** (for visualizing trends)

## How to Run the Project
1. Clone this repository.
2. Install the required libraries:
   ```sh
   pip install pandas google-api-python-client matplotlib seaborn
   ```
3. Replace `API_KEY` in the script with your YouTube Data API key.
4. Run the Python script to fetch data and generate insights.
   ```sh
   python youtube_analysis.py
   ```

## Future Improvements
- Expanding the analysis to multiple countries.
- Performing sentiment analysis on video comments.
- Automating data collection using cloud-based pipelines.

## Author
- **Gayatri Latkar**

---
This project provides valuable insights into YouTube trends, helping content creators make data-driven decisions. 🚀


