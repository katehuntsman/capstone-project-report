# Going Viral: Predicting Social Media Post Virality Through Engagement Metrics

**Author:** Kate E. Huntsman  
**Affiliation:** Northwest Missouri State University, Maryville MO 64468, USA  
**Email:** S577328@nwmissouri.edu

---

## Create/Activate Virtual Environment
```
python3 -m venv .venv
source .venv/bin/activate
```

## Abstract

This project looks at what makes social media posts go viral. We used data like likes, shares, comments, post type, and posting time to train some machine learning models that try to guess if a post will be viral or not. Virality here means the post’s views go over a certain number. The data was cleaned and explored before training models like Logistic Regression and Random Forest. We checked how well the models did using accuracy and F1 score. The results could help marketers and creators figure out how to get more engagement.

**Keywords:** social media analytics, virality prediction, machine learning, engagement metrics, data science

---

## Introduction

This project tries to predict whether a social media post will go viral based on how people engage with it. Going viral matters a lot to content creators and marketers who want to reach more people and have a bigger impact. Studies suggest posts that make people feel something or offer useful info tend to get shared more [Berger 2012](#references). Knowing what helps posts spread can improve how people manage their social media.

The data comes from a Kaggle dataset called *Viral Social Media Trends and Engagement Analysis* [Soundankar 2023](#references). It has info like likes, comments, shares, post type, category, and time when the post was made.

The main steps were cleaning the data, exploring it for patterns, creating new features, and training models to predict viral posts. This work adds to existing research about social media engagement [Chen 2023](#references).

There are some limits, like not having the actual post text or images (hashtags, pictures) and not accounting for how social media platforms decide what to show people.

**Full report:** [Overleaf project link](https://www.overleaf.com/read/trvpsqhftbyp#fe18e8)  
**Code repository:** [GitHub link](https://github.com/katehuntsman/capstone-project-report)

---

## Problem Definition

The goal is to tell if a post will go viral or not, based on engagement data. We define viral as having views above a certain threshold, so it’s a yes/no kind of prediction.

---

## Data Collection

We used the Kaggle dataset *Viral Social Media Trends and Engagement Analysis*. It contains post data like views, likes, shares, comments, categories, and when posts were published.

---

## Data Preparation

We cleaned the data by removing missing info and duplicates. Categories were turned into numbers, and timestamps were converted into date and time features. We also made a new label showing if a post is viral or not.

---

## Exploratory Data Analysis

We explored the data to see how likes, shares, and comments vary across different post types, categories, and times. We used charts like histograms and boxplots to find trends.

---

## Feature Engineering

We made some new features, such as:

- Grouping posts into viral or non-viral based on view counts
- Creating dummy variables for post types and categories
- Extracting hour of day and day of week from posting times

---

## Modeling and Evaluation

We trained two models: Logistic Regression and Random Forest. We tuned them using GridSearchCV and checked their performance with accuracy, precision, recall, F1 score, and confusion matrices.

---

## Results

The best model was *[insert model name]* with an F1 score of *[insert score]*. The most important things for predicting virality were:

- Number of shares
- Number of likes
- Time of day the post was made

It seems posts made around *[insert time]* have a higher chance to go viral.

---

## Conclusion and Future Work

This project shows that just looking at engagement data can help predict if a post will go viral. In the future, adding info like post text, images, or how platforms decide what to show could make predictions better.

---

## Project Workflow

![Project Workflow](figures/project_workflow.png)

*Figure: Project workflow showing the main steps: data collection, cleaning, feature building, modeling, and evaluation.*

---

## Resources & Links
- Dataset: [Kaggle – Viral Social Media Trends](https://www.kaggle.com/datasets/atharvasoundankar/viral-social-media-trends-and-engagement-analysis)  
- Overleaf Report (View Only): https://www.overleaf.com/read/trvpsqhftbyp#fe18e8
- GitHub Repo: https://github.com/katehuntsman/capstone-project-report

---

## Citations
Berger, J. (2012). Contagious: How to Build Word of Mouth in the Digital Age. Simon & Schuster. Available at: https://jonahberger.com/wp-content/uploads/2013/02/ViralityB.pdf

Soundankar, A., et al. (2023). Viral Social Media Trends and Engagement Analysis. Kaggle Dataset. Available at: https://www.kaggle.com/datasets/soundankar/viral-social-media-trends-and-engagement-analysis

Chen, X., et al. (2023). Machine Learning Approaches to Social Media Engagement. Journal/Conference.

Nair, R., et al. (2005). Understanding Virality and Information Spread in Social Networks. PLoS One. Available at: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11699135/