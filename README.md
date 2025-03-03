# Heart Disease Data Analysis Project

**Introduction**

This project uses a heart disease dataset to explore the relationships between various features and the occurrence of heart disease. It applies data exploration techniques, visualizes correlations and distributions, and builds a machine learning model (Gaussian Naive Bayes classifier) to predict heart disease likelihood.

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

**Draw correlation matrix**

A correlation heatmap is a great way to visualize which features are most correlated with the target variable and with each other. This helps in identifying redundant features and understanding relationships better.

![Image](https://github.com/user-attachments/assets/8430a095-4ba6-4c7f-87cc-5a4ef75b5214)

From the correlation heatmap, we would focus on features that show a strong correlation with the target variable (target). Features like cp, age, chol, thalach, trestbps, and exang usually show a significant correlation with the target variable based on medical research.

**Target distribution**

The countplot shows the frequency of heart attacks (1) versus no heart attack (0). This helps to quickly assess the class distribution of the target variable. 

![Image](https://github.com/user-attachments/assets/96b316b5-b63a-4697-944a-34e19fd21337)

**Target vs sex distribution**

Gender is an important factor in health-related studies, as it can influence the likelihood of heart attacks. This visualization helps to compare the heart disease distribution across genders, allowing us to easily see if one gender is more affected than the other.

![Image](https://github.com/user-attachments/assets/3e652b91-feba-4d1f-9ccf-e10772c4f36a)

**Age distribution**

The histplot is used to show how age is distributed, with a Kernel Density Estimate (KDE) curve highlighting trends. The age feature is important for analyzing health conditions like heart disease, as age can significantly impact risk. This visualization helps to understand the age demographics of the dataset and any patterns related to heart disease occurrences.

![Image](https://github.com/user-attachments/assets/701b63a4-83f8-45e1-ad98-6148d860b569)

**Chol distribution**

Cholesterol is a key factor in cardiovascular health, making it important to explore its distribution across both groups. This plot helps to identify the spread, central tendency, and potential outliers in cholesterol levels for each group, offering insights into the relationship between cholesterol levels and heart disease.

![Image](https://github.com/user-attachments/assets/6b0fb084-4d81-408b-b127-3f92fd94f51c)

**CP distribution**

Chest pain type is an important feature in heart disease diagnosis, so understanding its distribution across the dataset helps to assess which types of pain are more common.

![Image](https://github.com/user-attachments/assets/fb2f3fe1-5f40-49c7-a1de-4be342fe1a2a)

**Relation between 'age' and 'thalach' (maximum heart rate)**

This plot allows for an easy comparison between individuals with and without heart disease, offering insights into whether age impacts maximum heart rate and if heart disease influences this relationship.

![Image](https://github.com/user-attachments/assets/e66f3bad-80eb-4b58-b8c4-5bc1b9bce8ba)


**Feature and Target Variable Separation**

After impoting essential libraries for modeling and evaluation. The script separates the features (X) and the target variable (y) from the dataset.

**Data Splitting**

In the next part, data is splitted into training (80%) and testing (20%) sets using train_test_split with a fixed random seed for reproducibility.

**Model initialization, training and prediction**

The GaussianNB model is used from scikit-learn to perform classification. It trains the model on X_train and y_train using the fit() method, then makes 

predictions on X_test with the predict() method to generate the predicted labels (y_pred).

**Model evaluation**

This step evaluates the model's performance by calculating the accuracy using accuracy_score(), which is printed as a percentage. 

The confusion matrix is generated and visualized with a heatmap to show the counts of true positives, false positives, etc.

![Image](https://github.com/user-attachments/assets/f0fc49b4-c758-4ab8-81d3-d0451c1bd0a5)

Finally, a classification report is printed, providing detailed metrics like precision, recall, and F1-score.


