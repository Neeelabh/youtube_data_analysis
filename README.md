

---

# YouTube Sentiment Analysis Project

## Overview
This project analyzes multiple YouTube channels to provide insights into their performance based on key metrics such as **subscribers, views, likes, and comments**. The analysis is done using **Python** in a **Jupyter Notebook** environment, employing the **YouTube Data API v3** and web scraping techniques for data extraction. The goal of this project is to uncover patterns and sentiment trends across various YouTube channels, followed by an in-depth analysis of one particular channel, evaluating its performance based on **monthly uploads** of videos.

## Features
- **Multi-Channel Analysis**: Examination of different YouTube channels with respect to their subscriber count, views, likes, and comments.
- **Single Channel Focus**: A deeper analysis of a specific YouTube channel, with an emphasis on its monthly uploads and associated performance metrics.
- **Data Extraction**: Leveraging the YouTube Data API v3 and web scraping to gather channel-specific and video-specific data.
- **Data Visualization**: Utilizing **Seaborn** to create meaningful visualizations that showcase trends and insights.
- **Data Analysis**: Employing **Pandas** for data wrangling and statistical analysis to derive actionable insights from raw YouTube data.

## Project Structure
```
.
├── data/                 # Folder containing extracted raw data
├── notebooks/            # Jupyter Notebooks used for the analysis
├── visualizations/       # Folder containing generated plots and graphs
├── README.md             # Project documentation
└── requirements.txt      # Python package dependencies
```

## Tools & Libraries Used
- **Programming Language**: Python
- **Data Extraction**: 
  - YouTube Data API v3
  - Web scraping (for additional or unavailable data points)
- **Data Analysis**: 
  - Pandas: for data manipulation, cleaning, and analysis
- **Data Visualization**: 
  - Seaborn: for creating plots, bar charts, and heatmaps
- **Notebook Environment**: 
  - Jupyter Notebook: for step-by-step analysis and visualization

## Data Extraction
The data required for the analysis was gathered using the **YouTube Data API v3**. The API allows access to various YouTube metrics like subscriber count, total views, likes, and comments at both channel and video levels. Additionally, web scraping was utilized to supplement the data where the API had limitations.

### How to Use the YouTube Data API:
1. **Set up API credentials**: You need to create an API key from the Google Cloud Console and enable the YouTube Data API v3.
2. **Request Data**: Use the API to query specific YouTube channels or videos. Example queries can include getting basic statistics of a channel or retrieving comments from a particular video.
3. **Store Data**: Collected data is stored in structured formats (CSV/JSON) and processed with **Pandas** for further analysis.

## Data Analysis
The following steps were taken during the analysis:
1. **Channel Performance Comparison**:
   - Channels were compared based on their number of subscribers, total views, likes, and comment counts.
   - Insights were drawn from correlations between the metrics to understand channel growth patterns and audience engagement.

2. **Single Channel Monthly Performance**:
   - A selected YouTube channel was analyzed based on its monthly video uploads.
   - Key metrics such as views per upload, engagement rates (likes and comments), and upload frequency were visualized to track performance over time.

### Key Visualizations:
- **Subscriber Growth Trends**: Line plots to show the growth trajectory of subscribers.
- **Engagement Heatmaps**: To visualize the relationship between video views, likes, and comments.
- **Monthly Upload Performance**: Bar plots representing the number of videos uploaded each month alongside corresponding view counts.
  
## Setup Instructions
To run this project locally, follow the steps below:

### Prerequisites:
- Python 3.x
- Jupyter Notebook

### Installation:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/youtube-sentiment-analysis.git
   cd youtube-sentiment-analysis
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Obtain a YouTube Data API key:
   - Go to the [Google Cloud Console](https://console.cloud.google.com/)
   - Enable the **YouTube Data API v3**
   - Generate an API key and replace the placeholder in the notebook with your API key.

4. Open the Jupyter Notebook and run the cells sequentially:
   ```bash
   jupyter notebook
   ```

## Results
Through this analysis, the following insights were gained:
- Certain channels with high engagement (likes, comments) didn’t necessarily have the largest subscriber bases, indicating strong community interaction despite smaller audiences.
- The in-depth analysis of a single YouTube channel revealed that channels posting consistently across months tended to show stable viewership and engagement trends, while inconsistent upload patterns led to fluctuating viewer activity.

## Future Work
Potential enhancements to this project include:
- **Sentiment Analysis**: Perform sentiment analysis on the comments to understand viewer emotions towards content.
- **Deeper NLP Integration**: Use Natural Language Processing to analyze video titles, descriptions, and comments for more nuanced insights.
- **Time-Series Forecasting**: Leverage predictive models to forecast future subscriber growth and video performance trends based on historical data.

## Conclusion
This project demonstrates how the **YouTube Data API** can be effectively used to analyze YouTube channel performance and extract actionable insights. The combination of data analysis and visualization provides a comprehensive view of how channels perform over time, helping content creators and marketers optimize their strategies.

---

