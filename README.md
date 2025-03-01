# Heart Disease Data Analysis Project

**Introduction**

This project uses a heart attack dataset to explore the relationships between various features and the occurrence of heart attacks. It applies data exploration techniques, visualizes correlations and distributions, and builds a machine learning model (Gaussian Naive Bayes classifier) to predict heart attack likelihood.

**Libraries and dataset**

The project kicks off by importing essential Python libraries for data analysis, including Pandas, Matplotlib, and Seaborn. The dataset, which contains information related to heart disease, is loaded for exploration and analysis.

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

**Display top rows of the dataset**

 The first five rows of the dataset are displayed using df.head(), providing an initial overview of the columns and their values.

**Get information about the dataset and find shape of it**

Next step provides an overview of the dataset's structure, including its dimensions (rows and columns) and basic summary information such as data types and non-null counts.

**Check for null values**

Both isnull() and isna() are used to identify missing values and sum() aggregates the count of missing entries per column. This helps assess data completeness before analysis. Fortunately, the dataset is found to be free of any null values.

**Check for duplicated values**

The duplicated() function checks for duplicate rows and this code filters and displays them, helping ensure data quality by identifying any repeated entries.

**Get overall statistics about the dataset:**

It provides essential metrics such as mean, standard deviation and quartiles, helping to understand the distribution and variability of the data. This summary offers a quick snapshot of the central tendencies and spread within the dataset.

 
