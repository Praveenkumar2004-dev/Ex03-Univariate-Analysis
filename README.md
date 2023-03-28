# Ex03-Univariate-Analysis

## AIM
To read the given data and perform the univariate analysis with different types of plots

## EXPLANATION
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## ALGORITHM
## Step 1
Read the given data.
## Step 2
Get the information about the data.
## Step 3
Remove the null values from the data.
## Step 4
Mention the datatypes from the data.
## Step 5
Count the values from the data.
## Step 6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## PROGRAM
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)

sns.countplot(x='Postal Code',data=df)

sns.distplot(df["Postal Code"])

sns.histplot(x='Postal Code',data=df)

## OUTPUT
DATA

![1](https://user-images.githubusercontent.com/119559827/228139022-54f4703f-cf21-47a9-b37c-658f888eb495.png)

DATA HEAD

![2](https://user-images.githubusercontent.com/119559827/228139374-dd2de1a6-b022-4be5-9f89-317c17e0be26.png)

DATA INFORMATION

![3](https://user-images.githubusercontent.com/119559827/228139550-7022bc72-b296-4579-8b7c-498b91339897.png)

DATA DESCRIBE

![DES](https://user-images.githubusercontent.com/119559827/228139763-1fa75bd5-e764-4b64-855f-eecfac319800.png)

DATA NULL VALUES

![NULL](https://user-images.githubusercontent.com/119559827/228140010-a6a7f19c-bb75-4ea9-9ff9-15a3d290e9a0.png)

DATA'S DATATYPES

![def](https://user-images.githubusercontent.com/119559827/228140368-0a9dae96-f0f2-421f-b05a-725980343ca7.png)

DATA'S VALUECOUNT

![postal](https://user-images.githubusercontent.com/119559827/228140570-e3204320-b22a-4ea2-a8c5-e4630ce4a83e.png)

BOXPLOT

![6](https://user-images.githubusercontent.com/119559827/228140656-7a09bee2-8d23-4414-83fd-9f4b6a87033c.png)

COUNTPLOT

![7](https://user-images.githubusercontent.com/119559827/228140713-3e6e26be-9e26-4e6c-9fd2-42c93d73f42e.png)

DISTRIBUTION PLOT

![8](https://user-images.githubusercontent.com/119559827/228140801-61d1d2e5-3899-430c-81f9-25cbb0c63efb.png)

HISTOGRAM PLOT

![9](https://user-images.githubusercontent.com/119559827/228140953-5f8322a5-cbf1-4a62-a7a8-3b9b5ccaff82.png)

## RESULT
Thus we have read the given data and performed the univariate analysis with different types of plots.
















