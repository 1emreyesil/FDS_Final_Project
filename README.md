# Depression Detection Using Behavioral Data and PHQ4 Score

This repository contains a machine learning project aimed at forecasting depression levels based on a combination of activity data, survey results, and mobile data. The dataset used includes information such as user activity, sleep data, and survey results (specifically the PHQ-4 test) to predict depression levels. The project includes various stages such as data preprocessing, exploratory data analysis (EDA), feature engineering, dimensionality reduction using PCA, and model application. In this project our main dataset was [College Experience Study Dataset](https://www.kaggle.com/datasets/subigyanepal/college-experience-dataset)

The present repository contains the solutions to the FDS Final Project for the year 2024/2025.

#### Collaborators (Group 30):
- Emre Yesil ([1emreyesil](https://github.com/1emreyesil)) 
- Recep Yılmaz ([Rezeb](https://github.com/Rezeb))
- Nihal Yaman Yılmaz ([Nihal-yaman](https://github.com/Nihal-yaman))
  
## Files Overview
- `main.ipynb`: This is the main notebook containing the solutions to the project, along with a command to install the required packages.
- `dataset (Folder)`: This folder include the dataset csv files that we used in our porject.

## Project Abstract: Depression Detection Using Behavioral Data and PHQ4 Score


The project is organized as follows:

1. **Data Preprocessing**  
   In this step, data cleaning and feature selection were performed. Features that showed the least correlation with depression scores were removed based on correlation matrix analysis and OLS (Ordinary Least Squares) reports. This helped improve the model's efficiency and focus on relevant features.

2. **Exploratory Data Analysis (EDA)**  
   EDA was performed to understand the distribution of the features, identify any missing values, and understand the relationships between the features and the target variable (depression score). Various visualizations, including histograms, box plots, and correlation heatmaps, were used to explore the dataset.

3. **Feature Engineering**  
   New features were derived from the existing data to better capture the patterns related to depression. Additionally, feature scaling techniques were applied to normalize the data, ensuring that the features are comparable in terms of scale.

4. **Principal Component Analysis (PCA)**  
   PCA was applied to reduce the dimensionality of the dataset, making it easier to visualize and interpret the data. This step helped to identify the most important components that contribute to the variance in the data.

5. **Model Application**  
   Several machine learning models were applied to predict depression scores. To handle class imbalance, SMOTE (Synthetic Minority Over-sampling Technique) was used to oversample the minority class. Hyperparameter tuning using GridSearch was also conducted to optimize model performance, with a focus on finding the best learning rate and number of leaves for tree-based models.

6. **Conclusion**  
   The models were evaluated using different performance metrics, including accuracy, precision, recall, and F1-score. The results indicated that the feature engineering and model selection steps significantly impacted model performance. Further improvements could be made by enhancing the dataset with additional features and applying more advanced algorithms such as deep learning.

## PHQ-4 Test

The **PHQ-4** (Patient Health Questionnaire-4) is a four-item screening tool designed to assess the severity of depression and anxiety. The test consists of the following questions:

1. **Little interest or pleasure in doing things?**
2. **Feeling down, depressed, or hopeless?**
3. **Feeling nervous, anxious, or on edge?**
4. **Not being able to stop or control worrying?**

These questions are using for calculating PHQ-4 Score. In this project first 2 question of them were used to calculate the depression score in this project, which is a key target variable for model training and evaluation.
