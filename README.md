# COVID-19 Twitter Analysis 📊

## Overview
This project explores COVID-19 discourse on Twitter by analyzing **179,108 tweets** collected between **July and August 2020**. The dataset, sourced from Kaggle, was preprocessed and analyzed to extract key insights into public sentiment, misinformation trends, and engagement patterns.  

## Objectives  
✔ **Sentiment Analysis:** Categorizing tweets as positive, negative, or neutral using machine learning models.  
✔ **Hashtag & Topic Analysis:** Identifying the most common hashtags and trending discussions.  
✔ **Geographic Tweet Distribution:** Mapping tweet volumes by country and analyzing tweet density.  
✔ **User Engagement Trends:** Investigating how factors like follower count and verification status impact engagement.  
✔ **Misinformation Tracking:** Exploring the role of verified vs. non-verified users in spreading COVID-19 information.  

## Dataset Information  
The dataset contains **179,108** tweets and **13 features**, including:  
- **User Metadata**: Name, location, followers, friends, verification status.  
- **Tweet Details**: Text, hashtags, source, engagement metrics.  
- **Temporal Data**: Date and time of posting.  

## Data Processing & Feature Engineering  
🔹 Cleaned and preprocessed raw text by removing duplicates, emojis, special characters, and unwanted symbols.  
🔹 Converted boolean features (`is_retweet`, `user_verified`) to numeric format for consistency.  
🔹 Extracted **date components (day, month, time)** to analyze tweet volume over time.  
🔹 Created a new column to handle **URLs separately** from tweet text.  

## Research Questions  
📌 **What are the most common hashtags used in COVID-19-related tweets across different regions?**  
📌 **Can sentiment analysis identify trends in public opinion?**  
📌 **How do tweet volumes change over time, and what events cause spikes?**  
📌 **Is there a correlation between a user’s followers/friends count and tweet engagement?**  

## Data Visualization  
📊 **Tweet Volume Over Time**: A time-series graph showing spikes in COVID-19 discussions.  
📍 **Heatmap of Geographic Tweet Density**: Identifying the most active locations.  
📈 **User Engagement Metrics**: Scatter plots exploring correlations between user verification status and engagement.  
🔎 **Top Hashtags & Topics**: Bar charts and network graphs highlighting trending hashtags.  
🥧 **Tweet Volume by Verification Status**: A pie chart showing that **87.1% of tweets came from verified users**.  

## Model Implementation  
✔ **Naïve Bayes & Logistic Regression** for sentiment classification.  
✔ **Neural Networks (Sequential Model)** for deep learning-based sentiment analysis.  
✔ **TF-IDF Vectorization** for text feature extraction.  
✔ **Voting Classifier (Ensemble Learning)** for improved classification accuracy.  

## Results & Insights  
📌 **India, USA, and Australia** had the highest number of COVID-19-related tweets.  
📌 **Misinformation hubs** were identified by tracking the **"source"** field in tweets.  
📌 **Verified users (87.1%)** contributed the majority of tweets, highlighting the role of authoritative accounts.  
📌 **Sentiment analysis revealed shifts** in public sentiment, aligning with major pandemic events.  

## Installation & Usage  
### 🔧 Prerequisites  
- Python 3.x  
- Jupyter Notebook / Google Colab  
- Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `nltk`, `wordcloud`, `folium`, `networkx`, `tensorflow`  

### 🚀 Setup  
1️⃣ Clone the repository:  
```bash
git clone https://github.com/your-github-username/COVID19-Twitter-Analysis.git
cd COVID19-Twitter-Analysis
