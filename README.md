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

<h2 align="center"> <small>FIGURE 1.1(Total number of missing values)</small> </h2>
  
>Result: Figure 1 showing a series of the number missing in values from four columns of the Salary dataset.

<h2 align="center"> 

![12](https://github.com/user-attachments/assets/bad59397-35a1-4635-9781-c6419bde4a00) 

</h2>



<h2 align="center"> <small>FIGURE 1.2(Row with Missing value)</small> </h2>

 
>Result: Figure 1.2 shows the 5 rows that contain missing values across any of the columns.


#### **This involves identifying and dealing with missing data in your dataset. Common techniques including**:



>>1	Removing records with missing values.



<h2 align="center"> 
 
 ![image](https://github.com/user-attachments/assets/908d47e8-4ff8-4f14-9d2b-78c719e07b2a)

<h2 align="center"> <small>FIGURE 1.3(Cleaning the Dataset)</small> </h2>

Figure 1.3 codes ensures that any missing values (NaNs) in the four specified columns (Age, Gender, Years of Experience, Salary) are replaced with the most common value (mode) for each column. This is a common technique when handling categorical or numerical data with missing values, where replacing missing data with the mode can help maintain the distribution of the dataset.

>>2 Saving the cleaned Dataset.

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/93d7de5d-4fc6-4861-826c-156eb8cf82f8)

<h2 align="center"> <small>FIGURE 1.4(Clean Dataset)</small> </h2>

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/053e362a-53d8-4e4a-ba68-5780666d63e9)

<h2 align="center"> <small>FIGURE 1.4(FILE LOCATION)</small> </h2>


2.	Label Encoder 
>A Label Encoder in scikit-learn is used to convert categorical labels (text or other non-numeric values) into numerical form. This is particularly useful in machine learning models, which generally require inputs to be in numeric form.


<h2 align="center"> 

![image](https://github.com/user-attachments/assets/5ccc796c-fc84-4a94-89eb-37b247cc8854)



<h2 align="center"> <small>FIGURE 2.1.(Changing Variables to Numeric)</small> </h2>

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
