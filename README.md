# Evaluating Elegance: Sentiment Analysis in European Luxury Hotel Reviews

This repository contains the official code, datasets, and visualizations for the research paper "Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews," published by IEEE for the Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025).

## 📄 Publication

* **Paper:** Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews
* **Conference:** Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025)
* **Publisher:** IEEE

## 📝 Abstract

This research investigates customer sentiment in reviews for luxury European hotels sourced from Google Reviews and Tripadvisor. The project implements a machine learning pipeline to preprocess and analyze review text, applying various classification algorithms (e.g., Logistic Regression, Random Forest, SVM) to model and evaluate sentiment as Positive, Negative, or Neutral. The study also includes geographical visualization of the hotels and countries included in the dataset using interactive maps.

## 🗂️ Repository Structure
## 🛠️ Methodology

The complete analysis is contained within the `uncensored_thesiswork.ipynb` Jupyter Notebook. The workflow is as follows:

1.  **Data Loading:** The dataset (`hotel_reviewssentiments.csv`) is loaded for analysis.
2.  **Text Preprocessing:** A series of cleaning steps are applied to the raw review text:
    * Dropping null values
    * Lowercasing
    * Tokenization (NLTK)
    * Removal of punctuation, stopwords, emojis, and numbers
    * Stemming (NLTK PorterStemmer)
3.  **Feature Extraction:** The cleaned text is vectorized using **TF-IDF (Term Frequency-Inverse Document Frequency)**.
4.  **Model Training:** The dataset is split (80% train / 20% test) and the following machine learning models are trained:
    * Logistic Regression
    * Decision Trees
    * Random Forest
    * Support Vector Machine (SVM)
    * k-Nearest Neighbors (k-NN)
    * Gaussian Naive Bayes
5.  **Model Evaluation:** Performance is compared using **Accuracy**, **Precision**, **Recall**, and **F1-Score**.
6.  **Data Visualization:** Interactive maps are generated using **Folium** to plot the geographical locations of the hotels and countries in the dataset, saved as `.html` files.

## 🚀 How to Run

To replicate the analysis and regenerate the visualizations, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/al-foysal-tuhin/Evaluating-Elegance-Hotel-Reviews.git](https://github.com/al-foysal-tuhin/Evaluating-Elegance-Hotel-Reviews.git)
    cd Evaluating-Elegance-Hotel-Reviews
    ```

2.  **Install dependencies:**
    It's recommended to use a virtual environment. You will need to create the `requirements.txt` file first (see next section).
    ```bash
    pip install -r requirements.txt
    ```

3.  **Download NLTK data:**
    Run the following in a Python interpreter to download the necessary NLTK packages:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

4.  **Run the notebook:**
    Launch Jupyter Notebook and open `uncensored_thesiswork.ipynb`.
    ```bash
    jupyter notebook uncensored_thesiswork.ipynb
    ```
    You can run all cells to reproduce the model training and generate the `.html` map files.

## 📋 Requirements

You must create a `requirements.txt` file in your repository with the following content. These are the main libraries used in your notebook.

## 🗺️ Visualizations

The notebook generates two interactive maps, which are also saved in this repository:
* `hotels_world_map.html`: Plots the specific location of each hotel included in the study.
* `world_map_all14_countries.html`: Shows the 14 different countries from which hotel review data was collected.

You can download and open these `.html` files directly in any web browser to explore the maps.

## 📜 Citation

If you use this code or data in your research, please cite the original paper:

```bibtex
@inproceedings{[Tuhin_2025],
  author    = {[Al Foysal Tuhin}, [Rakhi Moni Saha}, [Adiba Masud}, [Tasnim Ara Shifa}, [Nusrat Jahan Mim}, [Sazia Sarmin},
  title     = {Evaluating Elegance: Sentiment Analysis In European Luxury Hotel Reviews},
  booktitle = {Proc. Annual International Conference on Data Science, Machine Learning and Blockchain Technology (AICDMB-2025)},
  year      = {2025},
  publisher = {IEEE}
}

