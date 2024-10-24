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

### **1.	Handle Missing Values**
   
 <h2 align="center"> 
  
![image](https://github.com/user-attachments/assets/8c1a99fb-feb7-4fe8-b4cc-4e9c62596bb9)


<h2 align="center"> <small>FIGURE 1.1:Total number of missing values</small> </h2>
  
Figure 1 showing a series of  number missing in values from four columns of the Salary dataset.

<h2 align="center"> 

![image](https://github.com/user-attachments/assets/035f86ca-7359-44c3-8cab-68a0474f6200)


</h2>



<h2 align="center"> <small>FIGURE 1.2:Row with Missing value</small> </h2>

 
Figure 1.2 shows the 5 rows that contain missing values across any of the columns.


### **2. Dealing with missing data in your dataset**


>>2.1	Removing records with missing values.


<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/1aa758d8-4c13-4c9c-9622-d31812b1a981)


<h2 align="center"> <small>FIGURE 2.1:Removing Unnecessary Data</small> </h2>

Figure 2.1 codes ensures that any missing values (NaNs) in the four specified columns (Age, Gender, Years of Experience, Salary) are replaced with the most common value (mode) for each column. This is a common technique when handling categorical or numerical data with missing values, where replacing missing data with the mode can help maintain the distribution of the dataset.

>>2.2 Saving the cleaned Dataset.

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/93d7de5d-4fc6-4861-826c-156eb8cf82f8)

<h2 align="center"> 
 
![image](https://github.com/user-attachments/assets/053e362a-53d8-4e4a-ba68-5780666d63e9)

<h2 align="center"> <small>FIGURE 2.2:FILE LOCATION</small> </h2>

>>Figure 2.2 shows where the saved document can be found in a folder such as 'Documents/Projects'.

## **3. Converting categorical labels/text to numeric form.**

Label Encoder 
>A Label Encoder in scikit-learn is used to convert categorical labels (text or other non-numeric values) into numerical form. This is particularly useful in machine learning models, which generally require inputs to be in numeric form. Since gender is the only non-numeric value, this is the only thing that can be replaced 


<h2 align="center"> 

![image](https://github.com/user-attachments/assets/38ae0f3b-27e0-415b-aaf8-d54d03bdf8ff)


![image](https://github.com/user-attachments/assets/f82e822e-be92-49e3-8e7b-614f256df0ae)



<h2 align="center"> <small>FIGURE 3.1:Changing Variables to Numeric</small> </h2>

### **4. Map out the Excel file for easy reference, allowing you to understand what the numeric values represent**

<h2 align="center"> 

![image](https://github.com/user-attachments/assets/b502cff3-4c9b-4b59-9c39-195807244427)

<h2 align="center"> <small>FIGURE 4.1:EDUCATION AND JOB TITLE</small> </h2>

In Figure 4.1, Gender was not included due to the limited numerical values it provided. Instead, job title and education level were used, as they offer more reference values. 

<h2 align="center">


![image](https://github.com/user-attachments/assets/7fe137ce-ccff-4c27-b479-2246c2f7ed9d)


![image](https://github.com/user-attachments/assets/b234288b-a78c-4ac1-af60-cbdcddac9016)

<h2 align="center"> <small>FIGURE 4.1:Reference Value</h2>


Figure 4.2 shows the reference values of the numbers.Since it consists of 316 job titles, you can refer to the Excel file to view the reference values of the numbers.

Assigning a unique number category For Gender :

>o	Male == 1
>o	Female == 0











#### **MODEL IMPLEMENTATION**:


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
