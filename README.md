Workshop-Multivariate-analysis

Aim

To perform Multivariate EDA on the given data set.

##Explanation

Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

Algorithm

Step1

Import the built libraries required to perform EDA and outlier removal.

Step2

Read the given csv file.

Step3

Convert the file into a dataframe and get information of the data.

Step4

Return the objects containing counts of unique values using (value_counts()).

Step5

Plot the counts i

n the form of Histogram or Bar Graph.

Step6

Use seaborn the bar graph comparison of data can be viewed.

Step7

Find the pairwise correlation of all columns in the dataframe.corr()

Step8

Save the final data set into the file.


Types of bivariate analyis

1)Numerical & Numerical(Scatter plot)
2)Numerical & Categorical(Bar plot,Box plot,Dist plot)



Developed by : JOEL P

Registration Number : 212222230057

Code

```
import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()

```

Output

Data Head

![image](https://user-images.githubusercontent.com/118626456/229035857-949434ce-b505-4bca-b046-6f0d44992117.png)


Data Information

![image](https://user-images.githubusercontent.com/118626456/229036030-565a738e-45df-4a3e-bb76-79f17573f820.png)

Numerical & Numerical(Scatter plot)

![image](https://user-images.githubusercontent.com/118626456/229036157-6b8da167-db1a-4406-a24a-170aed40349f.png)

Numerical & Categorical(Bar plot)

![image](https://user-images.githubusercontent.com/118626456/229036200-33e50ec6-7e53-4d6e-ab40-cc89682c6b7f.png)

Non-Graphical method(correlation)

![image](https://user-images.githubusercontent.com/118626456/229036283-8e84ba1e-7fc5-4131-a3b2-6a8111c76880.png)

Result

Thus we have performed Multivariate EDA on the given data set.
