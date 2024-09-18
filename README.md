# Chart Toppers: Billboard Top 100 Songs

### Authors: Athena Ru, Khushmeet Chandi, Zaid Muqsit  
**Date: 2023-12-02**

## Overview

This project aims to analyze what makes songs successful on the Billboard Hot 100. Using data from Billboard and Spotify, we investigate the following questions:
1. What factors influence how long a song stays on the Billboard chart?
2. What determines how high a song peaks on the chart?
3. How have the characteristics of popular songs evolved across decades?

We build three models to explore these questions, with insights that may benefit artists, producers, and music industry professionals.

## Data

The data used in this analysis comes from two main sources:
- **Billboard Hot 100 charts**: Weekly song rankings from 1958 to 2021.
- **Spotify Web API**: Audio features of the songs, such as danceability, tempo, and popularity.

The merged dataset contains 12,055 observations, covering the period from August 9, 1958, to May 29, 2021.

## Models

### 1. Model 1: Predicting Longevity
A Random Forest model that predicts how many months a song will stay on the Billboard Top 100 based on features like danceability, Spotify popularity, tempo, and loudness.

### 2. Model 2: Predicting Peak Quantile
A Cumulative Logit model that predicts the chart quantile (top 25, 26-50, etc.) a song will peak in, based on factors like debut position, explicitness, genre, and popularity.

### 3. Model 3: Decade Classification
A Multinomial model that predicts the decade in which a song was released based on its audio features. This model helps highlight how musical trends and characteristics have changed over time.

## Key Findings

- **Spotify Popularity** is a consistent predictor across all models.
- Songs with higher debut positions and explicit lyrics are more likely to peak in higher chart quantiles.
- Over the decades, music has evolved with increasing energy, while loudness has stabilized.

## Methodology

The models were trained and tested on an 80/20 split of the data, and performance metrics such as accuracy and R² were calculated. We also explored variable importance and interaction effects to better understand the relationships between song features and chart performance.

## Visualizations

The repository includes several exploratory data analysis (EDA) plots, including:
- Longevity vs. Danceability
- Peak Quantile vs. Genre
- Energy, Danceability, and Loudness Trends Across Decades

## Conclusion

This project provides insights into what makes a song successful on the Billboard Hot 100 and how music trends have shifted over time. The models can be used by music industry professionals to better understand and predict song performance.
