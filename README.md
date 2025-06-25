# capstone-project-report

# Going Viral: Predicting Social Media Post Virality Through Engagement Metrics

## Overview
This project uses machine learning to predict the virality of social media posts based on user engagement metrics such as likes, shares, comments, and time of posting. The dataset comes from Kaggle and includes thousands of posts from various platforms with associated metadata.

The goal is to help content creators, marketers, and analysts understand what drives a post to go viral.

---

## Problem Statement
What makes a social media post go viral?  
By identifying key factors that influence engagement, we aim to:
- Analyze patterns across highly engaged posts.
- Predict virality using classification models.
- Recommend content strategies based on data-driven insights.

---

## Dataset
**Source:** [Viral Social Media Trends and Engagement Analysis (Kaggle)](https://www.kaggle.com/datasets/atharvasoundankar/viral-social-media-trends-and-engagement-analysis)  
**Author:** Atharva Soundankar  
**Accessed:** June 2025

The dataset includes:
- `post_type` (video, image, text, etc.)
- `likes`, `comments`, `shares`
- `views` (used to define virality)
- `category`, `time_posted`, and more

---

## Project Workflow
1. **Data Loading and Cleaning**
   - Handle missing values
   - Remove duplicates
   - Standardize formats

2. **Exploratory Data Analysis (EDA)**
   - Distribution of engagements
   - Correlations between metrics

3. **Feature Engineering**
   - Encode categorical variables
   - Create binary target: viral vs non-viral

4. **Modeling**
   - Logistic Regression
   - Random Forest Classifier
   - Evaluate using accuracy, F1, ROC-AUC

5. **Results & Insights**
   - Feature importance
   - Recommendations for content strategy

6. **Reporting**
   - Technical report written in LaTeX (Overleaf)
   - Visualizations and final metrics

---

## Limitations
- This project does not address algorithm-specific behavior of individual platforms (e.g., TikTok’s recommendation engine).
- No time-series forecasting is performed.
- The dataset may not fully capture content context (e.g., trends, hashtags, audio use).
- It assumes uniform exposure potential across all posts, which may not reflect platform biases.

---

## Resources & Links
- Dataset: [Kaggle – Viral Social Media Trends](https://www.kaggle.com/datasets/atharvasoundankar/viral-social-media-trends-and-engagement-analysis)  
- Overleaf Report (View Only): https://www.overleaf.com/read/trvpsqhftbyp#fe18e8
- GitHub Repo: https://github.com/katehuntsman/capstone-project-report

---

## Citations
- Soundankar, A. (2023). *Viral Social Media Trends and Engagement Analysis* [Dataset]. Kaggle. https://www.kaggle.com/datasets/atharvasoundankar/viral-social-media-trends-and-engagement-analysis  

