# solar_flares_classification
Solar flares classification using SciKitLearn supervised ML algorithms


# SVM_nonlinear_3labels_experiments
Trained SVM model on labeled data. 3 labels were used: no flare, weak flares, and strong flares. Only the no flare class was correctly classified. Therefore we decided to check how many weak flare data points there are. 


# Solar Flares Classification

## Introduction
This project focuses on the classification of solar flares using various data analysis and machine learning techniques. The goal is to predict the category of solar flares based on observational data.

## Project Structure
Here is an overview of the key files and directories in this project:

- `1_observation_plot.ipynb`: Notebook for plotting observations related to solar flares.
- `Comparing_Models.ipynb`: Notebook for comparing different machine learning models.
- `Correlating&Labeling-Noise-Reduction.ipynb`: Notebook for data correlation, labeling, and noise reduction.
- `Normalized_Filtering.ipynb`: Notebook for applying normalized filtering techniques on the dataset.
- `README.md`: The README file for the project (this document).
- `SVM_nonlinear_3labels_experiments.ipynb`: Notebook for experimenting with non-linear SVM models with 3 labels.
- `Solar_flares_data.ipynb`: Notebook for exploring solar flares data.
- `data_labeling_7labels.ipynb`: Notebook for labeling the data with 7 different labels.
- `flares_data_cleaning.ipynb`: Notebook for cleaning the solar flares data.

## Installation
To set up this project locally, you'll need to have Python installed, along with Jupyter Notebooks or JupyterLab. Clone this repository and install the required dependencies:

```bash
git clone https://github.com/yourgithubusername/solar_flares_classification.git
cd solar_flares_classification
pip install -r requirements.txt  # Assuming there's a requirements.txt file
