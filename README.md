Reddit Public Social Data Analytics Bot
A non-commercial, personal-use bot for analyzing public Reddit data to learn about community trends and sentiment.
Purpose
This is a personal, non-commercial project designed for learning and private research only. It uses the Reddit API to:
Read public posts and comments from topic-specific subreddits
Analyze basic community trends (e.g., popular topics, activity patterns)
Perform simple sentiment analysis on public discussions
Aggregate anonymized data for personal learning purposes
This bot will not be distributed to other users and strictly complies with Reddit’s API Terms of Service and rate limits.
Features
Fetch public posts/comments from specified subreddits
Basic trend analysis (post frequency, top keywords)
Simple sentiment scoring for discussions
Local data storage (no public sharing of raw data)
Built-in rate limit compliance
Installation
Prerequisites
Python 3.8+
A Reddit account (for API access)
Reddit API credentials (client ID, client secret, user agent)
Setup
Clone or download this repository
Install dependencies:
bash
运行
pip install praw pandas nltk
Create a config.py file in the project root with your Reddit API credentials:
python
运行
# config.py
REDDIT_CLIENT_ID = "your_client_id"
REDDIT_CLIENT_SECRET = "your_client_secret"
REDDIT_USER_AGENT = "your_user_agent (e.g., 'script:my_analytics_bot:v1.0 (by u/YourUsername)')"
Usage
Edit main.py to specify the subreddits you want to analyze:
python
运行
TARGET_SUBREDDITS = ["learnpython", "dataanalysis"]  # Example subreddits
Run the bot:
bash
运行
python main.py
Analyzed results will be saved locally as CSV files in the output/ directory.
Compliance & Terms
This project strictly adheres to Reddit’s rules:
Non-commercial use only: No monetization, no paid services
Public data only: No access to private messages, user profiles, or restricted content
Rate limit compliance: Built-in controls to avoid excessive API requests
No data sharing: All collected data is for personal use only and will not be distributed
Proper attribution: Follows Reddit’s API attribution requirements
License
This project is licensed under the 
MIT License
File
 for non-commercial, personal use only.
Disclaimer
This is a personal learning project and is not affiliated with or endorsed by Reddit. All use of the Reddit API is subject to Reddit’s 
Developer Terms of Service
File
.
