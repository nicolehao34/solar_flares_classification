# Detecting and CLassifying Flares in High-Resolution Solar Spectra with Supervised Machine Learning
Solar flares are a well-studied aspect of solar magnetic activity. Detecting and classifying solar flares will play a crucial role in studying the impact of stellar contamination caused by flares in exoplanet transmission spectra. In this paper, we present a standardized procedure to classify solar flares using supervised machine learning. Using a set of solar flares data from the NASA database and solar spectra from HARPS-N, we trained several supervised machine learning models and found the best performing supervised learning algorithm is a C-Support Vector Machine with non-linear kernels, specifically Radial Basis Function (RBF). The best-trained model, SVC with RBF kernel achieves an average aggregate accuracy score of 0.65, and categorical accuracy scores over 0.70 for the no flare and weak flares class. Testing the model showed that the model is able to detect and classify solar flares in completely new data with different characteristics and distributions from those of the training set. Future efforts could enhance the classification accuracy and explore the potential of alternative models, including deep learning approaches, and additional datasets, with a view to extending such a framework to exoplanet host stars.


# SVM_nonlinear_3labels_experiments
Trained SVM model on labeled data. 3 labels were used: no flare, weak flares, and strong flares. Only the no flare class was correctly classified. Therefore we decided to check how many weak flare data points there are. 


# Solar Flares Classification

## Introduction
This project focuses on the classification of solar flares using various data analysis and machine learning techniques. The goal is to predict the category of solar flares based on observational data.

## Project Structure
Here is an overview of the key files and directories in this project:

- `1_observation_plot.ipynb`: Plots observations related to solar flares.
- `Comparing_Models.ipynb`: Compares different machine learning models and evaluates their performance using confusion matrices and accuracy scores.
- `Correlating&Labeling-Noise-Reduction.ipynb`: Data correlation, labeling, and noise reduction.
- `Normalized_Filtering.ipynb`: Applies normalized filtering techniques on the dataset.
- `README.md`: The README file for the project (this document).
- `SVM_nonlinear_3labels_experiments.ipynb`: Experimenting with non-linear SVM models with 3 labels.
- `Solar_flares_data.ipynb`: Download the solar flares data.
- `data_labeling_7labels.ipynb`: Labels the solar flares data with 7 different labels. We initially used seven labels: strong flare start, during strong flare, strong flare end, weak flare start, during weak flare, weak flare end, no flare
- `flares_data_cleaning.ipynb`:  Basic data cleaning of the solar flares date set - getting rid of invalid and missing data.

## Installation
To set up this project locally, you'll need to have Python installed, along with Jupyter Notebooks or JupyterLab. Clone this repository and install the required dependencies:

```bash
git clone https://github.com/nicolehao34/solar_flares_classification.git
cd solar_flares_classification
pip install -r requirements.txt  
