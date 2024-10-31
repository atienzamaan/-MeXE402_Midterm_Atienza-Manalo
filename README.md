 # MeXE402_Midterm_Atienza-Manalo
#### Both Linear Regression and Logistic Regression are foundational techniques in machine learning used for different types of problems. While they share similarities in their structure, they are applied to distinct tasks and have different mathematical foundations. This repository will serve as our midterm exam that is designed to assess our understanding of Linear Regression and Logistic Regression through practical application on real-world datasets.

# Linear Regression
# **Introduction**
This dataset contains information about salaries, years of experience, and other relevant factors. It's a suitable dataset for predicting salaries based on experience using linear regression.
#### **Key Features**:
  - `Salary`:The corresponding salary of the employee (in dollars).
  - `Years of Experience`: The number of years an employee has worked in their field.
  - `Gender:`The gender of the employee (e.g., Male, Female, Non-binary).
  - `Education Level:` The highest level of education attained by the employee (e.g., High School, Bachelor’s Degree, Master’s Degree, Ph.D.).
  - `Job title`: The employee's position or title within their organization (e.g., Software Engineer, Data Analyst, Project Manager).
  -  `Age:` The age of the employee (in years).
#### **Dependent Variable**:
   - `Salary`:The corresponding salary of the employee (in dollars).
# **Objective of the Dataset**
The objective of the Salary Dataset is to analyze the relationship between salaries and years of experience and to build predictive models using linear regression. The primary goal is to predict an individual's salary based on their years of experience and other relevant factors. This can help in understanding salary trends, making informed salary forecasts, and identifying patterns between experience and earnings.
# **Linear Regression Analysis**

## Data Preprocessing

### **1.	Categorize job titles according to salaries from highest to lowest**
   
 <h2 align="center"> 
  
![image](https://github.com/user-attachments/assets/01b6e44b-0bb3-4818-9d14-311457efb18d)


<h2 align="center"> <small>Figure 1.1 Salary Range</small> </h2>
  
In Figure 1.1 Salary Range table shows the salary categorization from highest to lowest based on job title Salary range organizing wages based on job titles from highest to lowest simplifies data, for analysis purposes and assists in recognizing discrepancies and patterns in pay scales across roles within the organization.



### **2.Converting non-numerical to numerical values.**

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/55ddd932-ebe5-4241-bda6-039b81c31892)



<h2 align="center"> <small>Figure 2.1 NUMERICAL VALUE</small> </h2>

In Figure 2.1 using Excel's 'Find and Replace' feature to convert job titles and educational levels into numerical values enhances data consistency. This allows for more accurate pay distribution analysis, helping linear regression predictions become more precise.



### **3.References for Numerical Value.**

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/37130018-b23e-452c-9e73-db08b7c44393)

![image](https://github.com/user-attachments/assets/0b758e7f-ba2c-4aaf-a8b5-5978ab7e58c7)

<h2 align="center"> <small>FIGURE 3.1 LIST </small> </h2>

Figure 3.1 provides a comprehensive list of reference values associated with the numerical data used in the analysis. Due to the extensive nature of the dataset, it is recommended to consult the accompanying Excel file named "Salary_Data_Reference_Value" for a detailed reference of numerical values. 

### **4.Removing variables to improve accuracy by focusing on relevant data.**

<h2 align="center"> 

![image](https://github.com/user-attachments/assets/cef660e9-a479-4495-8cf9-2d2a1969f6f8)

<h2 align="center"> <small>FIGURE 4.1 REMOVING UNNCECESSARY DATA </small> </h2>

Figure 4.1 demostrate that removing age and gender can improve data accuracy by eliminating irrelevant or potentially biased information. This streamlines the dataset, focusing only on relevant variables, which enhances model performance and leads to clearer insights.

### **5.Check for missing values in each Rows and column. **


<h2 align="center"> 

![image](https://github.com/user-attachments/assets/eaec1bb6-5731-4ec1-b96d-a4d1a1c2a618)


<h2 align="center"> <small>FIGURE 5.1 MISSING VALUES </small> </h2>

In Figure 4.1 it is crucial, during data pre-processing where missing values are checked along the rows and columns. It identifies gaps in a dataset, and analysts go on to decide how such gaps or missing values in a dataset should be dealt with-imputed, dropped, or interpolated. Preserving data integrity is usually helped by handling missing values and generally improves the general quality and reliability of any analysis.

### **6.	Handling missing values**

<h2 align="center"> 

![image](https://github.com/user-attachments/assets/0bc2128b-c385-4d77-b15e-6ff014ba7eaa)

<h2 align="center"> <small>FIGURE 6.1 CLEANING THE DATASET </small> </h2>

In Figure 6.1 shows how to perform accurate cleaning of data to correct inaccuracies and inconsistencies, ensuring high data quality. This process involves handling missing values, removing duplicates, and standardizing formats. Automating these tasks improves efficiency and accuracy, leading to more reliable insights for analysis and decision-making.

# **MODEL IMPLEMENTATION**:


<h2 align="center">

 
![image](https://github.com/user-attachments/assets/83f3e0bc-d39b-4a19-9126-6bdb1a22bb83)


<h2 align="center"> <small> IMPORTING THE DATASET</small> </h2>

First, the panda’s library is imported as pd, which is a common convention. Then, the read_csv() function is used to load the CSV file named "Salary_Data_cleaned.csv" into a Pandas DataFrame named dataset. This Data Frame stores the data in a tabular format, making it easier to work with. Finally, the head () method is called on the dataset to display the first 5 rows of the DataFrame, providing a glimpse of the data's structure and content.</h2>

<h2 align="center">

![image](https://github.com/user-attachments/assets/3266886b-06c5-454c-9b86-a3a6ede99e51)

<h2 align="center"> <small> INPUTS AND OUPUTS</small> </h2>

The code effectively separates the dataset into two parts:
-	X: Contains the independent variables (features) that will be used to predict the salary.
-	y: Contains the dependent variable (target) that represents the salary values to be predicted.
This step is crucial in machine learning workflows as it prepares the data for training a model.

<h2 align="center">

![image](https://github.com/user-attachments/assets/9eabf698-97be-4010-9468-e02d5fa7e299)

<h2 align="center"> <small>TRAINING AND TEST SET</small> </h2>


The train_test_split function is imported from the sklearn.model_selection module. This module provides various tools for model selection and evaluation. The train_test_split function is called with the input features (X), the target variable (y), the desired test set size (test_size=0.2), and a random seed (random_state=0). 


•  Output: The function returns four sets: 


<h2 align="center">

![image](https://github.com/user-attachments/assets/7bebabbb-87f4-48e3-a614-53e0a5f4a9e3)

<h2 align="center">X_train: Contains the features of the training set.</small> </h2>




<h2 align="center">

![image](https://github.com/user-attachments/assets/2244072a-f900-4b2e-ab1d-dfd4d8baf578)


<h2 align="center">	X_test: Contains the features of the testing set.</small> </h2>



<h2 align="center">

![image](https://github.com/user-attachments/assets/fc73a1a5-a60b-4e6d-a13f-c344a3fb0e19)


<h2 align="center">	y_train: Contains the target variable of the training set.</small> </h2>


<h2 align="center">

![image](https://github.com/user-attachments/assets/04200141-d4e5-4e4d-ae1d-94b97754f686)


<h2 align="center">y_test: Contains the target variable of the testing set..</small> </h2>



![image](https://github.com/user-attachments/assets/1450334d-e128-4b15-bbaa-502690c93c34)


This class provides a pre-built implementation of the linear regression algorithm. By creating an instance of this class, we effectively instantiate a linear regression model object. This model is now ready to be trained on the training data


<h2 align="center">

![image](https://github.com/user-attachments/assets/99926d4e-bd5a-4de1-a547-a5ecf2f23af5)

This line of code trains the linear regression model (model) on the training data. The fit method is like a function that takes the training features (X_train) and the corresponding target variable (y_train) as input. It teaches the model the best way to relate the features to the target.


<h2 align="center">
 
![image](https://github.com/user-attachments/assets/8d3f4c14-6868-42c6-8c7e-03a4719aff1c)

This line of code uses the trained model (model) to make predictions on the testing set (X_test). The predict method takes the input features of the testing set as input and returns the corresponding predicted target values. These predicted values are stored in the variable y_pred. 


<h2 align="center">

![image](https://github.com/user-attachments/assets/d8f6bad8-f5cb-4b84-bf87-0f263ab81a22)

![image](https://github.com/user-attachments/assets/ab59761b-dd77-4c7e-929c-5c5a5add3072)


•  This line of code uses the trained model (model) to make a prediction on a new data point. The input to the predict method is a 2D array containing the values for the input features of the new data point. In this case, the values are: age = 32, gender = 1, education level = 1, job title = 177, and years of experience = 5. 

•  Output: The predict method returns a predicted value, which in this case is 85745.79735184. This predicted value represents the estimated salary for the given data point based on the model's learned relationship between the input features and the target variable.

<h2 align="center">

![image](https://github.com/user-attachments/assets/23090e2d-4be9-42d6-b0cd-8bfcbee148b3)



This refers to using appropriate machine learning libraries to build and train the linear regression model. Commonly used libraries include:

- o	Scikit-learn for linear regression.
- o	Pandas and Numpy for data handling.
- o	Label Encoder for transforming categorical labels into numerical values.

Evaluation Metrics:
- 	Calculate R-squared
-  Mean Squared Error


## **The Significance of Coefficients in the Salary Dataset**:

The coefficients in a salary dataset provide valuable insights into which factors are most influential in predicting salary. They help identify patterns like gender pay gaps, the impact of education, and the value of experience, which can guide decisions related to compensation strategies, hiring practices, and addressing potential salary disparities. Here are the importance of coefficient under: 

#### **Age**:

The coefficient for age indicates how salary is expected to change with each additional year of age. In this dataset, it suggests that older individuals tend to earn more, likely due to the accumulation of experience or seniority.

#### **Gender**:

The gender coefficient measures the salary difference between males and females. In this dataset, there is no strong evidence of a significant gender-based salary gap.

#### **Education Levelt**:


The coefficient for education level reflects how salary is affected by increasing educational attainment. Individuals with higher levels of education tend to earn more, supporting the idea that education boosts earning potential.

#### **Job Title**:


This coefficient reflects salary differences across various roles. It indicates that certain job titles command higher or lower salaries, depending on the position's value in the job market.


#### **Years of Experience**:
Experience is one of the most critical factors. The coefficient for years of experience suggests that salary tends to increase with each additional year showing the rate of salary growth.



## **Model’s Predictive Power**:

The predictive power of your model can be assessed using metrics like R-squared (R²), Adjusted R-squared, and error measures. 

## **Key Metrics**:

1.	R-squared (R²): 0.6617
   
- R² explains how well the independent variables account for the variance in the dependent variable (salary).
- 66.17% of the variability in salary is explained by the model. This is moderately good, suggesting that your model captures most but not all of the salary determinants.

2.	Adjusted R-squared: 0.6603
- Adjusted R² adjusts for the number of predictors in the model. It penalizes the inclusion of irrelevant predictors that don't contribute to the model's predictive power.
- 66.03% means that even after accounting for the complexity of the model (number of predictors), the model still explains most of the variance in salary. The slight decrease from R² indicates that the model isn’t overfitting, as the number of predictors is appropriate.
  
Model Performance:

•	The R² and Adjusted R² values around 66% imply that your model has a moderate predictive power. While the model captures a large part of the variability in salary, there's still about 34% that remains unexplained. This could be due to other factors not included in the model, such as industry type, company size, performance incentives, or even location.

------

# Logistic Regression: Bank Marketing Campaign Analysis

## Introduction
- Logistic regression is a widely-used classification algorithm primarily applied to predict the probability of a binary outcome. This analysis uses logistic regression to forecast client behavior, specifically to predict whether a client will subscribe to a term deposit. The model explores relationships between client demographics, past campaign performance, and subscription likelihood.

## Dataset Description
- The dataset used is the Bank Marketing Dataset from a marketing campaign conducted by a Portuguese financial institution. It includes details about client attributes, previous marketing campaigns, and whether the client subscribed to a term deposit.

### Key Features
- **Client-related features**:
  - `age`: The client's age.
  - `job`: Job type (categorical).
  - `marital`: Marital status (categorical).
  - `education`: Education level (ordinal).
  - `balance`: Account balance, indicating available savings.
  - `housing`: Whether the client has a housing loan (binary).
  - `loan`: Whether the client has a personal loan (binary).

- **Campaign-related features**:
  - `duration`: Duration of the last call in seconds (indicator of engagement).
  - `campaign`: Number of contacts made during the campaign.

- **Output**:
  - `deposit` (target variable): Indicates if the client subscribed to a term deposit (`yes` or `no`).

### Objective
- The objective is to build a model that predicts whether a client will subscribe to a term deposit based on their attributes and previous campaign performance.

## Analysis

### Data Preprocessing
1. **Handling Missing Values**:
   - Identify and manage missing data by using methods like mean, median, or advanced techniques such as K-nearest neighbors.
  <img alt = "Python" height="200" src="https://github.com/user-attachments/assets/28cd84d0-7ce0-4234-9d42-0d04c9b1729d">
    <img alt = "Python" height="300" src="https://github.com/user-attachments/assets/e70fe7a8-d691-45dc-976e-cce1b994af5a">
 </p>
 
###
2. **Label Encoding**:
   - Assign unique numbers to categorical variables:
     #### Job Categories
     The following numerical values have been assigned to the job categories:
     - **Student** = 1
     - **Unemployed** = 2
     - **Retired** = 3
     - **Housemaid** = 4
     - **Blue-collar** = 5
     - **Services** = 6
     - **Technician** = 7
     - **Admin.** = 8
     - **Self-employed** = 9
     - **Management** = 10
     - **Entrepreneur** = 11

     #### Marital Status
     The marital status categories are encoded as follows:
     - **Married** = 3
     - **Single** = 2
     - **Divorced** = 1
     #### Housing Status
     The housing status is represented by:
     - **Yes** = 1
     - **No** = 0
     #### Loan Status
     The loan status is encoded as:
     - **Yes** = 1
     - **No** = 0
     #### Deposit Subscription
     The deposit subscription status is represented by:
     - **Yes** = 1
     - **No** = 0

### Model Implementation
The following libraries are used:
- **Pandas** (`import pandas as pd`):
  - Data manipulation and analysis, especially for reading, inspecting, and cleaning the dataset.
  - **Functions**:
    - `pd.read_csv()`: Loads the dataset.
      ![image](https://github.com/user-attachments/assets/ef6abf66-757d-4efe-aa2d-d96913640c39)
      ![image](https://github.com/user-attachments/assets/d7aeaaa2-fc9a-471b-9e06-20e05c1c1e1d)


    - `dataset.isnull()`: Checks for missing values.
      ![image](https://github.com/user-attachments/assets/b57f2a6f-7f7d-4c55-a61b-7b11be968ad0)

    - `fillna()`: Fills missing values.
      ![image](https://github.com/user-attachments/assets/6a16790c-6223-4bc7-947a-e12058cc4dbd)

    - `to_csv()`: Saves the cleaned dataset.
      ![image](https://github.com/user-attachments/assets/6af16652-28e1-46c1-888e-cd8cc132cff7)


- **Scikit-Learn**:
  - A machine learning library for preprocessing and modeling.
  - **Functions**:
    - `LabelEncoder`: Encodes categorical variables numerically.
      ![image](https://github.com/user-attachments/assets/0d86d4fa-d9a6-4d4c-a82f-f692367abd13)

    - `train_test_split`: Splits the dataset into training and testing sets.
      ![image](https://github.com/user-attachments/assets/678a95ec-4f0e-43c0-8ce3-c9fe27ff7830)

    - `StandardScaler`: Standardizes input features.
      ![image](https://github.com/user-attachments/assets/88e2602c-0c62-4a34-ad6d-29bd22e6436f)

    - `LogisticRegression`: Provides the logistic regression model.
      ![image](https://github.com/user-attachments/assets/694106e0-e569-40a2-92d0-dc444851fa75)

    - `confusion_matrix`, `accuracy_score`: Calculates model accuracy and displays the confusion matrix.
      ![image](https://github.com/user-attachments/assets/8d85bc28-7f79-4376-923e-6e359f1827bd)
      ![image](https://github.com/user-attachments/assets/aa95a74d-06e5-4993-9750-a6063e7e9b0f)



- **Matplotlib** (`import matplotlib.pyplot as plt`):
  - For data visualization, particularly for displaying the confusion matrix.
- **Seaborn** (`import seaborn as sns`):
  - A visualization library for creating heatmaps to visualize the confusion matrix.
 ![image](https://github.com/user-attachments/assets/2aaf4344-1b71-4080-bdb4-ca6c72aa9b75)


### Making Predictions
- The model can make predictions on individual data points to assess whether a client is likely to subscribe to a term deposit.
![Screenshot 2024-10-31 072203](https://github.com/user-attachments/assets/936c7677-9cf1-42c5-9a5a-191c671d2b0c)
![Screenshot 2024-10-31 072407](https://github.com/user-attachments/assets/6d3464e7-0cda-4255-b68f-829510a19497)

## Results
### Model Evaluation
- **Confusion Matrix**: Helps identify false positives and false negatives, important for understanding model performance.
<img align="center" src="https://github.com/user-attachments/assets/7d50172a-17b5-4ced-86b2-b9fa02e12343">
</p>

### 
- **Accuracy Formula**:
  </p>
  
  ![Screenshot 2024-10-31 072741](https://github.com/user-attachments/assets/9bf3dead-3746-4dcf-9f9b-5bf388bd8753)
  </p>
  
  ![Screenshot 2024-10-31 092057](https://github.com/user-attachments/assets/56d92dec-d624-44da-b547-aa3e02221f28)




- **Accuracy Score import from Sklearn**:
 ![Screenshot 2024-10-31 072828](https://github.com/user-attachments/assets/bf8d7bbb-b4e8-4260-a4de-9bec25a94ff9)
  - The model achieved an accuracy score of approximately 77.12%, indicating moderate effectiveness in predicting term deposit subscriptions.
 


## Discussion
- Logistic regression is relatively simple and highly interpretable. By examining the model coefficients, we can determine the influence of each feature on the likelihood of a client subscribing. This interpretability is valuable for understanding the relationship between client characteristics and campaign success.
    </p>
  With an accuracy of around 77.12%, the logistic regression model performs moderately well in predicting term deposit subscriptions. However, it has a noticeable rate of misclassification, specifically with false negatives. This can be a concern if the bank’s goal is to maximize subscription rates, as some clients who might subscribe could be missed by the model. Adjusting the model's focus depending on business priorities (either increasing recall for more true positives or precision to reduce false positives) can enhance its effectiveness in distinguishing between clients likely to subscribe and those who are not.

