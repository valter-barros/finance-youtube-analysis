# YouTube Personal Finance Channel Analysis

This project presents a comprehensive data analysis of the personal finance niche on YouTube. Leveraging the YouTube Data API, this study extracts and analyzes video and channel metrics from 10 prominent personal finance YouTube channels, encompassing over 8,000 publicly available videos.

## Project Overview

The primary goal of this project is to explore the evolving landscape of personal finance content on YouTube. It delves into various aspects, including viewership trends, the effectiveness of keywords and emotionally charged language in video titles, and the distinct impact of short-form video content (YouTube Shorts) on engagement.

## Data Collection

Data was collected using the YouTube Data API (Google Cloud). The dataset includes information on:

- **Channel Statistics**: Subscriber count, total views, and total videos uploaded for 10 selected personal finance channels.
- **Video Metrics**: Titles, descriptions, publication dates, view counts, like counts, and comment counts for over 8,000 individual videos.

## Data Preparation and Cleaning

The raw data underwent a rigorous preparation and cleaning process, which involved:

- Converting data types for numerical metrics (views, likes, comments, subscribers, total videos) to integers.
- Transforming `publishedAt` to datetime objects and `duration` to timedelta objects for time-series analysis.
- Handling missing values and removing irrelevant columns (e.g., `favouriteCount`).
- Categorizing videos into 'short-form' (YouTube Shorts, ≤3 minutes) and 'long-form' for comparative analysis.

## Exploratory Data Analysis (EDA)

The exploratory phase provided key insights into the dataset's characteristics:

- **Summary Statistics**: Detailed summaries of channel and video metrics (mean, median, sum, max) were generated and formatted for readability.
- **Channel-wise Analysis**: Metrics were aggregated by channel to understand individual channel performance and engagement ratios (like ratio, comment ratio).
- **Time-Series Analysis**: Monthly trends in video uploads and median views were analyzed to observe the dynamic nature of content consumption in the finance space.

## Key Questions & Analysis

The project addressed three main questions using statistical analysis and visualizations:

1. **Impact of Popular Keywords**  
   Investigated whether the use of common words and bigrams (two-word sequences) in video titles influences engagement metrics like view counts. Sentiment analysis was performed to identify common words and bigrams in video titles.

2. **Influence of Extreme and Subjective Language**  
   Examined the correlation between the polarity (emotional charge) and subjectivity of video titles and video engagement (views, likes, comments).

3. **Behavior of Short-Form Content**  
   Compared the performance and engagement patterns of short-form videos (YouTube Shorts) against traditional long-form videos, analyzing differences in like ratios, comment ratios, and overall trends since the global launch of YouTube Shorts. A regression model was also used to analyze the impact of various factors on video views.

## Technologies Used

- **Python**: The core programming language for data extraction and analysis.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **TextBlob**: For sentiment analysis of video titles.
- **Matplotlib & Seaborn**: For data visualization and plotting.
- **Statsmodels**: For statistical modeling, including OLS regression.

## Conclusion and Future Work

The analysis provided valuable insights into the personal finance content landscape on YouTube, highlighting trends in content creation, audience engagement, and the specific impact of short-form videos.

Future work could involve integrating additional real-world financial data to investigate potential correlations between economic downturns and the emotional tone of video titles, as people might seek more financial guidance online during such periods.
