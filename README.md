# Predicting Food Insecurity Through Temporal & Spatial Analysis

A machine learning project investigating whether **temporal and spatial socioeconomic data can be used to predict food insecurity across U.S. counties**.

Food insecurity is influenced by a complex combination of economic, health, demographic, and environmental factors. This project uses historical county-level data to model food insecurity and evaluate how different machine learning approaches perform when predicting future outcomes.

## Research Question

**Can historical socioeconomic, demographic, health, and environmental data be used to predict county-level food insecurity?**

The project approaches this problem as a **spatiotemporal prediction task**, using historical observations to predict food insecurity in subsequent years.

## Dataset

The dataset contains information from **3,142 U.S. counties**.

The models were trained using data from **2018–2022** and evaluated on actual food insecurity outcomes from **2023**.

The project incorporates 12 variables spanning socioeconomic, demographic, health, and environmental characteristics:

* College Graduation
* Obesity Rate
* Median Household Income
* Food Environment Index
* Uninsured Rate
* Poverty Rate
* Single-Parent Households
* Housing Problems
* Elderly Population
* Female Population
* Total Population
* Unemployment Rate

## Models

Several approaches were evaluated:

* **Convolutional Neural Network (CNN)**
* **Long Short-Term Memory Network (LSTM)**
* **ARIMA**

These models were compared based on their ability to predict county-level food insecurity.

## Results

The CNN achieved the strongest predictive performance among the evaluated models.

| Model |       MAE |
| ----- | --------: |
| CNN   | **0.025** |
| LSTM  |     1.197 |
| ARIMA |     1.899 |

The results suggest that the CNN was particularly effective at capturing patterns in the dataset.

## Feature Analysis

To investigate which variables contributed most strongly to predictions, the project uses **leave-one-variable-out permutation analysis**.

Each variable is removed or disrupted and the resulting change in model performance is analyzed. This provides a way to examine the importance of individual socioeconomic and demographic factors rather than treating the model as a complete black box.

## Application

The research was also developed into an application that translates model predictions into an interpretable **food insecurity risk score**.

The application categorizes predicted risk into several levels and provides data-driven information that can be used to identify areas experiencing greater levels of food insecurity.

The system also generates potential policy recommendations based on the factors associated with elevated risk.

## Technologies

* Python
* Machine Learning
* Deep Learning
* CNNs
* LSTMs
* ARIMA
* Pandas
* NumPy
* Data Visualization
* Spatiotemporal Analysis
* Statistical Analysis

## My Role

I designed and implemented the machine learning pipeline, including data preparation, model development, evaluation, and feature-importance analysis. I also developed the prediction application used to make the research more accessible and interpretable.

## Research

This project was developed as an independent research project and was submitted for publication.

## Code Availability

The complete implementation includes research and application components that cannot currently be publicly released. This repository therefore documents the methodology, experiments, results, and publicly shareable portions of the project without exposing restricted source code or data.

## Author

**Shaurya Singh**

Undergraduate Researcher
The University of Texas at Austin
