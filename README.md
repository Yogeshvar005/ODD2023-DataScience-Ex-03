# Ex03-Univariate-Analysis

# Aim:

To read the given data and perform the univariate analysis with different types of plots.

# Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:

# Step1:

Read the given data.

# Step2:

Get the information about the data.

# Step3:

Remove the null values from the data.

# Step4:

Mention the datatypes from the data.

# Step5:

Count the values from the data.

# Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:

# (1) Diabetes.csv

```py
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
sns.distplot(df["Glucose"])
sns.histplot(x="Glucose",data = df)
df.kurtosis()
sns.boxplot(x="Glucose",data=df)
```

# (2) SuperStore.csv

```python
df2 = pd.read_csv("/SuperStore.csv")
df2.head()
df2.isnull().sum()
df2['Postal Code'] = df2["Postal Code"].fillna(df2['Postal Code'].mode()[0])
df2.isnull().sum()
df2.dtypes
df2.describe()
df2['Sales'].value_counts()
sns.boxplot(x="Sales",data=df2)
sns.countplot(x="Sales",data=df2)
sns.distplot(df2['Sales'])
sns.histplot(x="Sales",data=df2)
df2.skew()
sns.distplot(df2["Postal Code"])
sns.histplot(x="Postal Code",data = df2)
df2.kurtosis()
sns.boxplot(x="Row ID",data=df2)
```

# OUTPUT:

# DIABETES.csv
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/4a20b495-3296-4f3d-9275-6a15ebf95e0c)


## INFO

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/6f5cefa7-9f71-4b33-9937-d037c96885b9)


## ISNULL.SUM
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/8b21b379-d93f-4c92-a35c-e8033de5e5f0)



## DTYPES
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/b7d80f6d-1e73-4f4c-a4b3-a69a836e29a2)



## DESCRIBE

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/31352467-c30b-414c-ba11-f56bea9ca833)


## VALUECOUNTS
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/fc68c6bd-a73b-46a5-afb1-035f0672d670)



## BOXPLOT

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/119dde87-84ef-44ea-8207-6a3810ad1101)


## COUNTPLOT
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/8a267088-5c4a-4af0-acb6-ee9b195fc728)


## DISTPLOT
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/c5bcd4e0-4ba2-445e-9911-6cfc1ab8b63d)


## HISTPLOT

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/1cd24b28-0d81-4b62-9f97-abd039a712f4)


## SKEW
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/a5299bbd-ce94-42cc-b796-e5a1c0f909a6)


## DISTPLOT SKEW

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/0fe35b45-189e-47dd-86ea-af4399a577f1)


## HISTPLOT SKEW

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/dc4a0b45-486f-45c2-b28e-60be0e256df3)


## KURTOSIS
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/2a4c7742-0649-45fd-a53f-0a477275fadf)



## BOXPLOT KURTOSIS

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/7a40444d-c6e9-4e6c-aa73-b96ff7fa086f)


# SUPERSTORE.csv

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/55b1d3c7-771e-46ad-929f-5f6a83688016)

## ISNULL.SUM
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/c464cba8-16ee-41a2-9d69-97aeb9b8decd)



## AFTER CLEANING

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/00638c2e-47e1-4f8a-aca5-31acf9bb02ef)


## DTYPES
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/389972c3-0865-483f-914a-f3d354736dc0)



## DESCRIBE

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/9bd959a1-6ac8-41bd-b15f-7ec308e57d99)


## VALUECOUNTS

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/fd400bde-648a-4f92-981d-3d46a5b73d06)


## BOXPLOT

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/8be7a836-84de-4d4c-82ef-9640b511d71b)


## COUNTPLOT
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/1aaca139-01a7-4db7-b8a7-cf5469995c57)


## DISTPLOT
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/2071ba59-d274-4b37-904f-55bc11f1c483)



## HISTPLOT

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/10772d93-088c-4b22-afa5-e7c037ec08e9)


## SKEW
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/c1eda4fc-bab1-43ac-938b-61d9e9d34e8a)


## DISTPLOT SKEW

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/6a44c8b0-2f33-4f33-88a6-060ccc1c86a4)


## HISTPLOT SKEW

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/7cbbc236-b661-40f9-8698-a4012a569b20)


## KURTOSIS
![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/9de0694e-73bd-4fca-a5bf-87d493c5b660)



## BOXPLOT KURTOSIS

![image](https://github.com/Yogeshvar005/ODD2023-DataScience-Ex-03/assets/113497367/780638a3-adf6-4158-b152-25eda0c9f858)


# RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.
