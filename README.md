# Detecting and Classifying Flares in High-Resolution Solar Spectra with Supervised Machine Learning

Solar flares are a well-studied aspect of solar magnetic activity. Detecting and classifying solar flares plays a crucial role in studying the impact of stellar contamination caused by flares in exoplanet transmission spectra. In this project, we present a standardized procedure to classify solar flares using supervised machine learning. Using a dataset of solar flares from the NASA database and solar spectra from HARPS-N, we trained several supervised machine learning models. The best-performing supervised learning algorithm is a C-Support Vector Machine with non-linear kernels, specifically Radial Basis Function (RBF). The best-trained model, SVC with RBF kernel, achieves an average aggregate accuracy score of 0.65 and categorical accuracy scores over 0.70 for the no flare and weak flares classes. Testing the model showed that it can detect and classify solar flares in completely new data with different characteristics and distributions from those of the training set. Future efforts could enhance classification accuracy, explore alternative models (including deep learning approaches), and incorporate additional datasets to extend such a framework to exoplanet host stars.

Thank you for supporting our work! Here's the link to our paper in the Astrophysical journal: https://iopscience.iop.org/article/10.3847/1538-4357/ad5be3

---

## Project Structure

Here is an overview of the key files, directories, and their primary functions:

- **`1_observation_plot.ipynb`**: 
    - Visualizes solar flare observations.
    - Key functions:
        - `plot_solar_flare_distribution()`: Plots the distribution of flare categories.
        - `visualize_time_series()`: Displays time-series data for solar flare activity.

- **`Comparing_Models.ipynb`**: 
    - Compares the performance of different machine learning models.
    - Key functions:
        - `train_models()`: Trains multiple models on the dataset.
        - `evaluate_models()`: Evaluates models using confusion matrices and accuracy scores.
        - `plot_model_comparison()`: Visualizes model performance comparisons.

- **`Correlating&Labeling-Noise-Reduction.ipynb`**: 
    - Performs data correlation analysis, labeling, and noise reduction.
    - Key functions:
        - `correlate_features()`: Identifies correlations between features.
        - `label_data()`: Labels the dataset with appropriate flare categories.
        - `reduce_noise()`: Applies noise reduction techniques to clean the data.

- **`Normalized_Filtering.ipynb`**: 
    - Applies normalized filtering techniques to preprocess the dataset.
    - Key functions:
        - `normalize_data()`: Normalizes the dataset for consistent scaling.
        - `apply_filtering()`: Filters out irrelevant or noisy data points.

- **`README.md`**: 
    - The README file for the project (this document).

- **`SVM_nonlinear_3labels_experiments.ipynb`**: 
    - Experiments with non-linear SVM models using three labels.
    - Key functions:
        - `train_svm_model()`: Trains an SVM model with a non-linear kernel.
        - `analyze_weak_flare_distribution()`: Analyzes the distribution of weak flare data points.

- **`Solar_flares_data.ipynb`**: 
    - Downloads and preprocesses the solar flares dataset.
    - Key functions:
        - `download_data()`: Fetches solar flare data from the NASA database.
        - `preprocess_data()`: Prepares the data for analysis and modeling.

- **`data_labeling_7labels.ipynb`**: 
    - Labels the solar flares data with seven different categories.
    - Key functions:
        - `generate_labels()`: Creates labels for strong flare start, during strong flare, strong flare end, weak flare start, during weak flare, weak flare end, and no flare.

- **`flares_data_cleaning.ipynb`**: 
    - Cleans the solar flares dataset by removing invalid and missing data.
    - Key functions:
        - `clean_data()`: Removes invalid or missing entries from the dataset.
        - `validate_cleaned_data()`: Ensures the cleaned dataset is ready for analysis.

---

## Installation

To set up this project locally, you'll need Python installed, along with Jupyter Notebooks or JupyterLab. Clone this repository and install the required dependencies:

```bash
git clone https://github.com/nicolehao34/solar_flares_classification.git
cd solar_flares_classification
pip install -r requirements.txt
```

---

## Future Work

- Enhance classification accuracy by exploring alternative machine learning models, including deep learning approaches.
- Incorporate additional datasets to improve model generalization.
- Extend the framework to classify solar flares in exoplanet host stars.

