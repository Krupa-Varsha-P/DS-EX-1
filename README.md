# Ex:-01(DATA CLEANSING)

## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

## EXPLANATION
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

## ALGORITHM
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

## PROGRAM
```python3
import pandas as pd 
df=pd.read_csv("Data_set.csv") 
print(df) 
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0]) 
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0]) 
df['original_network']=df[ 'original_network'].fillna(df['aired_on'].mode()[0]) 
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean()) 
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean()) 
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median()) 
df.head()
df.info()
df.isnull().sum()
import pandas as pd 
df=pd.read_csv("Loan_data.csv") 
print(df) 
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['Loan_ID']=df['Loan_ID'].fillna(df['LoanAmount'].mode()[0]) 
df.head()
df['Dependents']=df['Dependents'].fillna (df['Dependents'].mode()[0]) 
df.head()
df['Gender']=df['Gender'].fillna (df['Gender'].mode()[0]) 
df.head()
df['Education']=df['Education'].fillna (df['Dependents'].mode()[0]) 
df.head()
df['Self_Employed']=df['Self_Employed'].fillna (df['Self_Employed'].mode()[0]) 
df.head()
df['LoanAmount']=df['LoanAmount'].fillna (df['LoanAmount'].mean()) 
df.head()
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean()) 
df.head()
df['Credit_History']=df['Credit_History'].fillna (df['Credit_History'].median()) 
df.head()
df.info()
f.isnull().sum()
```
## OUTPUT
![Screen Shot 2023-08-29 at 7 26 14 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/b42e6c02-5197-4751-ae1f-f75ecab2949a)
![Screen Shot 2023-08-29 at 7 26 28 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/464f9950-031e-46f2-889c-7dab8a5b077f)
![Screen Shot 2023-08-29 at 7 26 44 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/6170160b-9963-4383-b1c7-e34af9e6ee9d)
![Screen Shot 2023-08-29 at 7 26 53 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/1f32698b-536f-4725-9f0a-be8bb069da56)
![Screen Shot 2023-08-29 at 7 27 12 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/71bb5f81-ab1a-4c16-9e61-99fb58b53445)
![Screen Shot 2023-08-29 at 7 27 25 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/efca49fb-3fa1-4962-9ba2-ed822ca918ee)
![Screen Shot 2023-08-29 at 7 28 01 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/614d64be-cc7c-4073-849d-8777eca8e90d)
![Screen Shot 2023-08-29 at 7 28 11 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/ee3c9ec4-2a4b-4107-a196-88fe4b85823e)
![Screen Shot 2023-08-29 at 7 28 29 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/ad8565a1-d228-4248-a15c-4663b239c0f9)
![Screen Shot 2023-08-29 at 7 28 46 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/b1163e05-e7a1-46d5-a233-d951dcdad6aa)
![Screen Shot 2023-08-29 at 7 29 04 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/6d6369ed-68a6-4239-b841-390b87c8895e)
![Screen Shot 2023-08-29 at 7 29 19 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/53c3868e-3653-47a8-bd5d-54957e3fff79)
![Screen Shot 2023-08-29 at 7 29 30 PM](https://github.com/Krupa-Varsha-P/DS-EX-1/assets/100466625/f91e92a3-80dc-44ac-97a2-063c8d8dd422)
