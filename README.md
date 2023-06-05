# Ex-No-10-Data-science-process-on-complex-dataset-

# AIM:

To Perform Data Visualization on a complex dataset and save the data to a file

# EXPLANATION:

Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM:

STEP 1 
Read the given Data 
STEP 2 Clean the Data Set using Data Cleaning Process 
STEP 3 Apply Feature generation and selection techniques to all the features of the data set 
STEP 4 Apply data visualization techniques to identify the patterns of the data.

CODE
/* Data Visualization - Iris.csv

import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

df = pd.read_csv("/content/iris.csv")

df.head()

df.info()

df["variety"].value_counts()

sns.countplot(x='variety', data=df, )

plt.show()

sns.scatterplot(x='sepal.length', y='sepal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.scatterplot(x='petal.length', y='petal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.pairplot(df.drop(['Id'], axis = 1), hue='variety', height=2)

fig, axes = plt.subplots(2, 2, figsize=(10,10))

axes[0,0].set_title("Sepal Length")

axes[0,0].hist(df['sepal.length'], bins=7)

axes[0,1].set_title("Sepal Width")

axes[0,1].hist(df['sepal.width'], bins=5);

axes[1,0].set_title("Petal Length")

axes[1,0].hist(df['petal.length'], bins=6);

axes[1,1].set_title("Petal Width")

axes[1,1].hist(df['petal.width'], bins=6);

sns.heatmap(df.corr(method='pearson').drop(['Id'], axis=1).drop(['Id'], axis=0), annot = True);

plt.show()

# OUTPUT
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/b53ca970-3eeb-4403-b3f4-c52842b37a80)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/fb4212d8-112c-40f7-bfe3-bdebf176c0d1)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/beaa7406-7d4e-4408-aa56-e823abfda60b)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/55b648c3-bcae-47e9-a1b6-ff242514b133)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/dc5d65f3-4826-4b7b-9f5c-f7bd45bf8ba9)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/88286ec6-e220-474c-9c4f-91ea5eb17a3d)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/2afffe95-a32b-4395-9d67-75efb77e2cc9)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/50f9a69e-5915-44a6-abde-f03e311129e1)
![image](https://github.com/Naveen3640/Ex-No-10-Data-science-process-on-complex-dataset-/assets/95179990/e936fe71-6b66-4d2d-a10f-9a3bf73738fe)


# RESULT

Thus the Data Visualization for the given dataset had been executed successfully.
