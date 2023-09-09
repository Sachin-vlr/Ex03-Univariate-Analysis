# Ex03-Univariate-Analysis
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:
# Step 1:
Read the given data.

# Step 2:
Get the information about the data.

# Step 3:
Remove the null values from the data.

# Step 4:
Mention the datatypes from the data.

# Step 5:
Count the values from the data.

# Step 6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
NAME : SACHIN.C
REG NO. : 212222230125
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

df=pd.read_csv("/content/iris (1).csv")

df.nunique()
```
![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/35035f11-6b37-4fa4-8c92-7c0f57ad8cb2)

```python
df.head()
```
![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/b8a8fa97-c8e0-44af-93b8-1ba992f1c31d)

```python
df.tail()
```
![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/5150482b-4c52-42b5-8863-77b1a0d57e80)

```python
df.iloc[:,4].value_counts()
```
![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/7a22bb4e-9a1f-4a23-a2b2-32a067a5e5ae)

```python
for i in range(0,df.shape[1]):
  print("-----------",df.columns[i],"------------")
  print(df.iloc[:,i].value_counts())
  print("---------------------------------------")
```

![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/b76f1b3e-4f70-49af-9234-c42b5811d1e1)![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/0616f381-37bb-4c8c-a49e-ce23b706b0c2)![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/507dd369-5492-4f37-9203-d9a2060e8acc)![image](https://github.com/Sachin-vlr/Ex03-Univariate-Analysis/assets/113497666/a76e1f58-4328-4b84-b912-9fe4e36ad767)









