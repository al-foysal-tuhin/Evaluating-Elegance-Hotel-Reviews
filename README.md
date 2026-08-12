# 🏨 Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews

<p align="center">
  <img src="https://img.shields.io/badge/IEEE-Published%20Research-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="IEEE Published Research">
  <img src="https://img.shields.io/badge/NLP-Sentiment%20Analysis-8A2BE2?style=for-the-badge" alt="NLP Sentiment Analysis">
  <img src="https://img.shields.io/badge/Machine%20Learning-6%20Models-FF6F00?style=for-the-badge" alt="Machine Learning">
  <img src="https://img.shields.io/badge/Python-Data%20Science-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
</p>

<p align="center">
  <strong>Sentiment Analysis • Natural Language Processing • Machine Learning • European Luxury Hospitality • Geospatial Analytics</strong>
</p>

---

## ✨ Overview

**Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews** is an IEEE-published research project investigating customer sentiment within luxury hotel reviews across Europe.

The research applies a complete **Natural Language Processing (NLP) and Machine Learning pipeline** to hotel reviews sourced from **Google Reviews and Tripadvisor**, classifying customer feedback into:

- 🟢 Positive
- 🟡 Neutral
- 🔴 Negative

The project combines **text preprocessing, TF-IDF feature extraction, six machine learning classification algorithms, model evaluation, and interactive geographical visualization** to investigate sentiment patterns within the European luxury hospitality sector.

The complete analysis and experimental workflow are contained in the accompanying Jupyter Notebook.

---

## 📄 IEEE Publication

This research was published by **IEEE** as part of the:

**Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025)**

| | |
|---|---|
| 📚 **Paper** | *Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews* |
| 🏛️ **Publisher** | IEEE |
| 🎓 **Conference** | Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025) |
| 📅 **Year** | 2025 |
| 🔗 **IEEE Xplore** | [View Published Paper](https://ieeexplore.ieee.org/document/11277568) |

<p align="center">
  <a href="https://ieeexplore.ieee.org/document/11277568">
    <img src="https://img.shields.io/badge/📄%20READ%20THE%20PUBLISHED%20PAPER-IEEE%20Xplore-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="Read the IEEE Paper">
  </a>
</p>

---

## 📝 Abstract

This research investigates customer sentiment in reviews for luxury European hotels sourced from **Google Reviews and Tripadvisor**.

A machine learning pipeline was developed to preprocess and analyze review text, followed by the application and comparison of multiple classification algorithms, including **Logistic Regression, Decision Trees, Random Forest, Support Vector Machine, k-Nearest Neighbors, and Gaussian Naive Bayes**.

The models classify reviews into **Positive, Negative, and Neutral** sentiment categories and are evaluated using **Accuracy, Precision, Recall, and F1-Score**.

The study also incorporates **interactive geographical visualization** to explore the distribution of hotels and countries represented within the dataset.

---

## 🎯 Research Objectives

The research focuses on:

- 💬 Analyzing customer sentiment in European luxury hotel reviews.
- 🧹 Developing an NLP preprocessing pipeline for unstructured review text.
- 🔢 Converting textual reviews into numerical features using TF-IDF.
- 🤖 Training and comparing six machine learning classification algorithms.
- 📊 Evaluating model performance using multiple classification metrics.
- 🌍 Investigating the geographical distribution of hotels represented in the dataset.
- 🗺️ Creating interactive maps for geographical exploration.
- 🔬 Identifying effective machine learning approaches for hotel-review sentiment classification.

---

## 🧠 Research Pipeline

    ┌───────────────────────────────────┐
    │       Hotel Review Dataset        │
    │                                   │
    │   Google Reviews + Tripadvisor    │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │       Text Preprocessing          │
    │                                   │
    │ • Null Removal                    │
    │ • Lowercasing                     │
    │ • Tokenization                    │
    │ • Stopword Removal                │
    │ • Punctuation Removal             │
    │ • Emoji & Number Removal          │
    │ • Stemming                        │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │          TF-IDF Vectorizer        │
    │                                   │
    │   Text → Numerical Representation │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │          Train / Test Split       │
    │              80 / 20              │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │      Machine Learning Models      │
    │                                   │
    │ • Logistic Regression             │
    │ • Decision Tree                   │
    │ • Random Forest                   │
    │ • Support Vector Machine          │
    │ • k-Nearest Neighbors             │
    │ • Gaussian Naive Bayes            │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │         Model Evaluation          │
    │                                   │
    │ • Accuracy                        │
    │ • Precision                       │
    │ • Recall                          │
    │ • F1-Score                        │
    └──────────────────┬────────────────┘
                       │
                       ▼
    ┌───────────────────────────────────┐
    │       Geospatial Analysis         │
    │                                   │
    │          Interactive Folium       │
    │               Maps                │
    └───────────────────────────────────┘

---

## 🔬 Methodology

### 1. Data Loading

The analysis begins with the hotel review dataset:

`hotel_reviewssentiments.csv`

The dataset contains review information used for sentiment classification and geographical analysis.

### 2. Text Preprocessing

The raw review text is cleaned using a sequence of NLP preprocessing operations:

- Dropping null values
- Converting text to lowercase
- Tokenization using NLTK
- Removing punctuation
- Removing stopwords
- Removing emojis
- Removing numerical characters
- Stemming using the NLTK `PorterStemmer`

### 3. Feature Extraction

The processed review text is converted into numerical features using:

**TF-IDF — Term Frequency-Inverse Document Frequency**

TF-IDF provides the numerical representation required by the traditional machine learning classifiers.

### 4. Train/Test Split

The dataset is divided into:

- **80% Training Data**
- **20% Testing Data**

### 5. Model Training

Six classification algorithms are trained:

| Model | Classification Approach |
|---|---|
| **Logistic Regression** | Linear classification |
| **Decision Tree** | Tree-based classification |
| **Random Forest** | Ensemble learning |
| **Support Vector Machine** | Margin-based classification |
| **k-Nearest Neighbors** | Instance-based classification |
| **Gaussian Naive Bayes** | Probabilistic classification |

### 6. Model Evaluation

Each model is evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

Using multiple metrics provides a more complete understanding of model performance.

### 7. Geographical Visualization

The research also uses **Folium** to create interactive geographical visualizations of the hotels and countries represented in the dataset.

---

## 🤖 Machine Learning Models

The project evaluates six different approaches to sentiment classification:

    ┌─────────────────────────────────────┐
    │        Sentiment Classification     │
    └──────────────────┬──────────────────┘
                       │
          ┌────────────┼────────────┐
          │            │            │
          ▼            ▼            ▼
    Logistic       Decision      Random
    Regression       Tree        Forest
          │            │            │
          └────────────┼────────────┘
                       │
          ┌────────────┼────────────┐
          │            │            │
          ▼            ▼            ▼
         SVM          k-NN     Naive Bayes

The purpose is to compare different machine learning strategies rather than relying on a single classifier.

---

## 🗺️ Interactive Visualizations

The notebook generates two interactive HTML maps.

### 🌍 Hotel Locations

`hotels_world_map.html`

Displays the geographical locations of the individual hotels included in the study.

### 🌎 Country Distribution

`world_map_all14_countries.html`

Visualizes the **14 countries** represented in the hotel review dataset.

The generated HTML files can be opened directly in a web browser.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| 🐍 **Python** | Core programming language |
| 📓 **Jupyter Notebook** | Research and experimentation |
| 🧠 **Scikit-learn** | Machine learning and evaluation |
| 📝 **NLTK** | Natural Language Processing |
| 📊 **Pandas** | Data manipulation |
| 🔢 **NumPy** | Numerical computation |
| 📈 **Matplotlib** | Data visualization |
| 🗺️ **Folium** | Interactive geographical visualization |

---

## 📂 Repository Structure

    Evaluating-Elegance-Hotel-Reviews/
    │
    ├── 📓 uncensored_thesiswork.ipynb
    │
    ├── 📄 README.md
    │
    ├── 📜 LICENSE
    │
    ├── 📦 requirements.txt
    │
    ├── 🏆 Research Paper Certificate.pdf
    │
    ├── 🗺️ hotels_world_map.html
    │
    └── 🌍 world_map_all14_countries.html

### 🔑 Main Research File

`uncensored_thesiswork.ipynb`

This notebook contains the complete research workflow, including data preprocessing, feature engineering, model training, evaluation, and visualization.

---

## 🚀 How to Run

### 1. Clone the Repository

    git clone https://github.com/al-foysal-tuhin/Evaluating-Elegance-Hotel-Reviews.git

    cd Evaluating-Elegance-Hotel-Reviews

### 2. Create a Virtual Environment

#### Windows

    python -m venv venv

    venv\Scripts\activate

#### Linux / macOS

    python3 -m venv venv

    source venv/bin/activate

### 3. Install Dependencies

    pip install -r requirements.txt

### 4. Download Required NLTK Resources

Open Python and run:

    import nltk

    nltk.download('punkt')
    nltk.download('stopwords')

### 5. Launch the Notebook

    jupyter notebook uncensored_thesiswork.ipynb

Run the notebook cells to reproduce the research analysis, model training, evaluation, and geographical visualizations.

---

## 📦 Requirements

The repository includes a `requirements.txt` file containing the core Python dependencies used by the research.

    pandas
    numpy
    scikit-learn
    nltk
    matplotlib
    folium

Install all dependencies with:

    pip install -r requirements.txt

---

## 📊 Research Workflow

The complete analytical workflow can be summarized as:

    Raw Hotel Reviews
           ↓
    Data Cleaning
           ↓
    NLP Preprocessing
           ↓
    TF-IDF Feature Extraction
           ↓
    80/20 Train-Test Split
           ↓
    Six ML Classification Models
           ↓
    Accuracy / Precision / Recall / F1
           ↓
    Comparative Analysis
           ↓
    Geographical Visualization

---

## 📈 Reproducibility

The repository is organized around a reproducible research workflow:

**Data → Preprocessing → Feature Extraction → Model Training → Evaluation → Visualization**

The primary Jupyter Notebook contains the complete analytical implementation, allowing researchers and developers to inspect the methodology and reproduce the experiments.

---

## 🌍 Geospatial Analysis

In addition to sentiment classification, the project explores the geographical characteristics of the dataset.

The interactive visualizations provide two perspectives:

**Hotel-level analysis**

Shows the individual geographical locations of the hotels.

**Country-level analysis**

Shows the distribution of the dataset across the 14 represented European countries.

This geographical component complements the NLP analysis by providing spatial context to the review data.

---

## 🏆 Research Contribution

This project demonstrates the application of traditional machine learning and NLP techniques to customer-generated hotel reviews.

The research combines:

### 💬 Sentiment Analysis

Extracting customer sentiment from natural-language hotel reviews.

### 🤖 Machine Learning

Comparing six different classification algorithms.

### 📊 Model Evaluation

Using Accuracy, Precision, Recall, and F1-Score to compare performance.

### 🌍 Geospatial Analytics

Mapping hotels and countries represented in the dataset.

Together, these components provide a multi-dimensional analytical perspective on European luxury hospitality reviews.

---

## 📜 Citation

If you use this research, methodology, or repository in your academic or professional work, please cite the published paper:

    @inproceedings{Tuhin_2025,
      author    = {Al Foysal Tuhin and Rakhi Moni Saha and Adiba Masud and Tasnim Ara Shifa and Nusrat Jahan Mim and Sazia Sarmin},
      title     = {Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews},
      booktitle = {Proc. Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025)},
      year      = {2025},
      publisher = {IEEE}
    }

### 📄 IEEE Xplore

<p align="center">
  <a href="https://ieeexplore.ieee.org/document/11277568">
    <img src="https://img.shields.io/badge/IEEE%20Xplore-Read%20Paper-00629B?style=for-the-badge&logo=ieee&logoColor=white" alt="IEEE Xplore">
  </a>
</p>

---

## 📚 Research Materials

| Resource | Description |
|---|---|
| 📓 `uncensored_thesiswork.ipynb` | Complete research and ML workflow |
| 📦 `requirements.txt` | Project dependencies |
| 🏆 `Research Paper Certificate.pdf` | Research publication certificate |
| 🗺️ `hotels_world_map.html` | Interactive hotel-location map |
| 🌍 `world_map_all14_countries.html` | Interactive country-distribution map |

---

## 🔮 Future Research Directions

Potential extensions include:

- 🤖 Transformer-based sentiment analysis
- 🧠 BERT-based and deep-learning models
- ⭐ Aspect-based sentiment analysis
- 🏨 Hotel-specific sentiment comparison
- 🌍 Country-level sentiment comparison
- 📊 Interactive analytical dashboards
- 📈 Temporal sentiment analysis
- 🔎 Explainable AI
- 🧪 Expanded model benchmarking
- 🌐 Multilingual European hotel-review analysis

---

## 👨‍💻 Author

### **AL Foysal Tuhin**

**Data Analyst • Data Science • Machine Learning • NLP • Research**

<p align="center">
  <a href="https://github.com/al-foysal-tuhin">
    <img src="https://img.shields.io/badge/GitHub-al--foysal--tuhin-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/alfoysaltuhin">
    <img src="https://img.shields.io/badge/LinkedIn-Al%20Foysal%20Tuhin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
</p>

---

## ⭐ Support the Research

If you find this project useful:

⭐ Star the repository

📄 Read the published IEEE paper

🔗 Share the research with others interested in NLP, machine learning, sentiment analysis, or hospitality analytics.

---

## 📜 License

This project is licensed under the **Apache License 2.0**.

See the `LICENSE` file for the complete license terms.

---

<p align="center">

<strong>From customer reviews to machine learning insights.</strong>

<br><br>

🏨 &nbsp; 💬 &nbsp; 🧠 &nbsp; 🤖 &nbsp; 📊 &nbsp; 🌍 &nbsp; 📄

<br><br>

<strong>Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews</strong>

<br>

<em>IEEE Published Research • AICDMB-2025</em>

</p>
