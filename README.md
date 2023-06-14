# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE

import pandas as pd

df=pd.read_csv("Loan_data.csv")

print(df)

df.head(10)

df.info()

df.isnull()

df.isnull.sum()

df['Gender']=df['Gender'].fillna(df['Gender'].mode()[0])

df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0])

df['Self_Employed']=df['Self_Employed'].fillna(df['Self_Employed'].mode()[0])

df.head()

df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())

df.head()

df['Credit_History']=df['Credit_History'].fillna(df['Credit_History'].median())

df.head()

df.info()

df.isnull.sum()

# OUPUT

![242287987-591e4dee-d61d-4648-be2f-6bb5f7e0f854](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/8b19e673-4d71-42ca-9198-65fc3b257226)

![242288041-f38d18d9-2835-461f-b5f2-e32a8d66e1f6](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/6ed65d0f-45c2-4376-95ec-5b90df87598e)

![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/b015ffac-e64f-4ede-9.d6a-765475e80ac8)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/31e8e427-cbe6-4411-930e-7b435a64986c)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/a425833a-7eb0-4916-8afa-ee55eeff9f07)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/3829af86-9ab2-440d-bbca-79d5f295f42b)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/5ac77f15-44ad-4ee4-9dad-65b98b873d19)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/ee4faf07-d28d-45fd-b7a7-5e8122620fa4)


![image](https://github.com/Rajasree-321/Ex-01-Data-Cleaning/assets/96918911/b3111d65-3b72-442b-8ba3-da88d3bcbb08)

# RESULT:
 Thus, the given data is read, cleansed and the cleansed data is saved into file.
