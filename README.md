# 🏨 Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews

<p align="center">
  <img src="https://img.shields.io/badge/Research-IEEE%20Published-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="IEEE Published">
  <img src="https://img.shields.io/badge/Machine%20Learning-NLP-8A2BE2?style=for-the-badge" alt="Machine Learning">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/License-Apache%202.0-D22128?style=for-the-badge" alt="License">
</p>

<p align="center">
  <strong>Sentiment Analysis • Natural Language Processing • Machine Learning • European Luxury Hospitality • Geospatial Analytics</strong>
</p>

<p align="center">
  <a href="https://ieeexplore.ieee.org/document/11277568">📄 Read the IEEE Paper</a>
  •
  <a href="https://github.com/al-foysal-tuhin/Evaluating-Elegance-Hotel-Reviews">💻 Repository</a>
</p>

---

## ✨ About the Research

**Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews** is a research project investigating customer sentiment across reviews of luxury hotels in Europe.

The study applies a complete **Natural Language Processing (NLP) and Machine Learning pipeline** to hotel reviews collected from **Google Reviews and Tripadvisor**, classifying customer feedback into:

- 🟢 **Positive**
- 🔴 **Negative**
- 🟡 **Neutral**

Beyond sentiment classification, the research explores the **geographical distribution of luxury hotels and review data across Europe**, combining machine learning with interactive geospatial visualization.

The complete research workflow is implemented in the accompanying Jupyter Notebook.

---

## 📄 IEEE Publication

This research has been **published by IEEE** and presented at the:

**Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025)**

| Publication | Details |
|---|---|
| 📚 Title | *Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews* |
| 🏛️ Publisher | IEEE |
| 🎓 Conference | AICDMB-2025 |
| 📅 Year | 2025 |
| 🔗 Paper | [IEEE Xplore](https://ieeexplore.ieee.org/document/11277568) |

### 📖 Published Paper

<p align="center">

<a href="https://ieeexplore.ieee.org/document/11277568">
  <img src="https://img.shields.io/badge/📄%20Read%20Published%20Paper-IEEE%20Xplore-00629B?style=for-the-badge" alt="Read Published Paper">
</a>

</p>

---

## 📝 Abstract

This research investigates customer sentiment in reviews for luxury European hotels sourced from **Google Reviews and Tripadvisor**.

A machine learning pipeline was developed to preprocess and analyze review text, followed by the application and comparison of multiple classification algorithms, including **Logistic Regression, Decision Trees, Random Forest, Support Vector Machine, k-Nearest Neighbors, and Gaussian Naive Bayes**.

The study evaluates model performance using **Accuracy, Precision, Recall, and F1-Score** while also incorporating geographical visualization to explore the distribution of hotels and countries represented in the dataset.

---

## 🎯 Research Objectives

The project focuses on several key objectives:

- Analyze customer sentiment within European luxury hotel reviews.
- Develop an NLP preprocessing pipeline for unstructured review text.
- Transform textual reviews into machine-readable numerical features.
- Train and compare multiple machine learning classification models.
- Evaluate model performance using standard classification metrics.
- Investigate the geographical distribution of the hotel dataset.
- Generate interactive maps to visually explore the collected data.
- Identify an effective machine learning approach for hotel-review sentiment classification.

---

## 🧠 Machine Learning Pipeline

```text
                    ┌─────────────────────────┐
                    │   Hotel Review Dataset  │
                    │ Google Reviews +         │
                    │ Tripadvisor             │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │    Data Preprocessing   │
                    │ • Null Removal          │
                    │ • Lowercasing           │
                    │ • Tokenization          │
                    │ • Stopword Removal      │
                    │ • Emoji Removal         │
                    │ • Punctuation Removal   │
                    │ • Stemming              │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │      TF-IDF Vectorizer  │
                    │ Text → Numerical        │
                    │ Feature Representation  │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │     Train / Test Split  │
                    │       80% / 20%         │
                    └────────────┬────────────┘
                                 │
              ┌──────────────────┼──────────────────┐
              │                  │                  │
              ▼                  ▼                  ▼
        Logistic Regression   Decision Tree    Random Forest
              │                  │                  │
              ▼                  ▼                  ▼
             SVM                 k-NN          Naive Bayes
              │                  │                  │
              └──────────────────┼──────────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │    Model Evaluation     │
                    │ • Accuracy              │
                    │ • Precision             │
                    │ • Recall                │
                    │ • F1-Score              │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │   Geospatial Analysis   │
                    │      using Folium       │
                    └─────────────────────────┘
