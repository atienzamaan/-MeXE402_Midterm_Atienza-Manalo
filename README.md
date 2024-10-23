 # MeXE402_Midterm_Atienza-Manalo
#### Both Linear Regression and Logistic Regression are foundational techniques in machine learning used for different types of problems. While they share similarities in their structure, they are applied to distinct tasks and have different mathematical foundations. This repository will serve as our midterm exam that is designed to assess our understanding of Linear Regression and Logistic Regression through practical application on real-world datasets.

## Linear Regression
### **Introduction**
#### **Dataset Description**
This dataset contains information about salaries, years of experience, and other relevant factors. It's a suitable dataset for predicting salaries based on experience using linear regression.
#### **Key Features**:
  - `Salary`:The corresponding salary of the employee (in dollars).
  - `Years of Experience`: The number of years an employee has worked in their field.
  - `age:`:.
  - `status`: 
#### **Dependent Variable**:
   - `Salary`:The corresponding salary of the employee (in dollars).
### **Objective of the Dataset**
The objective of the Salary Dataset is to analyze the relationship between salaries and years of experience and to build predictive models using linear regression. The primary goal is to predict an individual's salary based on their years of experience and other relevant factors. This can help in understanding salary trends, making informed salary forecasts, and identifying patterns between experience and earnings.
### **Analysis**
## Data Preprocessing
1.	Handle Missing Values

   
 <h2 align="center"> 
  
![Screenshot 2024-10-23 153637](https://github.com/user-attachments/assets/9d7c88dd-dc1c-47de-95f4-16e1b4979168) 



<h2 align="center"> ##FIGURE 1
  

<h2 align="center"> Result:FIGURE 1 showing a series of the number missing in values from four columns of the dataset.
  
![12](https://github.com/user-attachments/assets/bad59397-35a1-4635-9781-c6419bde4a00)



<h2 align="center"> FIGURE 2 
  


<h2 align="center">Result: The code outputs the rows that contain missing values across any of the columns:



<h2 align="center">In the result shown, 5 rows are displayed with missing values in various columns like Age, Gender, Years of Experience, and Salary.



>This involves identifying and dealing with missing data in your dataset. Common techniques include:


>1.1	Removing records with missing values.

![13](https://github.com/user-attachments/assets/4b642287-9739-4de0-81ba-50988d832c5c)



>2.2	Imputing values using methods such as mean, median, or mode, or more advanced techniques like K-nearest neighbors.


2.	Label Encoder 
>A Label Encoder in scikit-learn is used to convert categorical labels (text or other non-numeric values) into numerical form. This is particularly useful in machine learning models, which generally require inputs to be in numeric form.


![14](https://github.com/user-attachments/assets/8a7a7bcc-b56a-4382-989f-96fb1054d423)

------

## Logistic Regression 
### **Introduction**
#### **Dataset Description**
##### The dataset used in this analysis is the **Bank Marketing Dataset** from a marketing campaign conducted by a Portuguese financial institution. The dataset contains information on client attributes, previous marketing campaign details, and whether the client subscribed to a term deposit.

#### **Key Features**:
- **Client-related features**:
  - `age`: The age of the client.
  - `job`: The type of job the client has (categorical).
  - `marital`: The client’s marital status (categorical).
  - `education`: The client’s level of education (ordinal).
  
- **Campaign-related features**:
  - `contact`: The type of communication used during the campaign.
  - `previous`: Number of contacts performed before this campaign.
  
- **Output**:
  - `y`: The target variable indicating whether the client subscribed to a term deposit (`yes` or `no`).

### **Objective of the Dataset**:
The objective is to build a model to predict whether a client will subscribe to a term deposit based on the client’s attributes and the previous campaign's performance.

---




##### Explanation
![image](https://github.com/user-attachments/assets/be9096cd-e27a-44e2-b681-33ca4e35f352)
##### Project Objectives:
