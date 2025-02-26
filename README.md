# Heart Disease Data Analysis Project

**Introduction**

This project uses a heart attack dataset to explore the relationships between various features and the occurrence of heart attacks. It applies data exploration techniques, visualizes correlations and distributions, and builds a machine learning model (Gaussian Naive Bayes classifier) to predict heart attack likelihood.

**Libraries and Dataset**

The project kicks off by importing essential Python libraries for data analysis, including Pandas, Matplotlib, and Seaborn. The dataset, which contains information related to heart disease, is loaded for exploration and analysis

Here’s a data dictionary for the Heart Attack Data Set presented in a table format:

| **Feature**         | **Description**                                                                 |
|---------------------|---------------------------------------------------------------------------------|
| **age**             | Age of the patient (in years).                                                   |
| **sex**             | Gender of the patient (1 = male, 0 = female).                                   |
| **cp**              | Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic). |
| **trestbps**        | Resting blood pressure (in mm Hg).                                               |
| **chol**            | Serum cholesterol level (in mg/dl).                                              |
| **fbs**             | Fasting blood sugar (1 = > 120 mg/dl, 0 = < 120 mg/dl).                          |
| **restecg**         | Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy). |
| **thalach**         | Maximum heart rate achieved (in bpm).                                           |
| **exang**           | Exercise induced angina (1 = yes, 0 = no).                                       |
| **oldpeak**         | Depression induced by exercise relative to rest (in mm).                        |
| **slope**           | Slope of the peak exercise ST segment (0 = upsloping, 1 = flat, 2 = downsloping). |
| **ca**              | Number of major vessels colored by fluoroscopy (0-3).                           |
| **thal**            | Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect).               |
| **target**          | Presence or absence of heart disease (1 = yes, 0 = no).                         |


**Display Top Rows of the Dataset**

 The first five rows of the dataset are displayed using df.head(), providing an initial overview of the columns and their values.

 
