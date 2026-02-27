# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
    import seaborn as sns
    import pandas as pd
    # Replace with your actual CSV file
    df = pd.read_csv('iris.csv')
    df.head()
    df.corr()
    sns.heatmap(df.corr(),annot=True,linewidths=1,linecolor="white")
    sns.jointplot(x='sepal_length',y='petal_length',data=df,kind='hist',color='purple')
    sns.jointplot(x='sepal_width',y='petal_width',data=df,kind='reg',color='gold')
    sns.pairplot(df,hue='petal_length',palette='Set1')
    sns.pairplot(df,hue='sepal_length',palette='Set2')
    sns.distplot(df['sepal_length'])
    sns.distplot(df['petal_length'],kde=False,bins=10,color='red')
    sns.countplot(x='petal_length',data=df)
    sns.countplot(y='sepal_width',data=df)
    ## Bar plot
    sns.barplot(x='sepal_length',y='sepal_width',data=df,color='cyan',edgecolor='black')
    sns.barplot(x='sepal_width',y='sepal_length',data=df,color='magenta',edgecolor='black')
    sns.boxplot(
    x='species',
    y='sepal_length',
    data=df,
    palette='Set1',
    boxprops=dict(edgecolor='black', linewidth=2),
    medianprops=dict(color='black', linewidth=2),
    whiskerprops=dict(color='black', linewidth=2),
    capprops=dict(color='black', linewidth=2)
      )
     sns.violinplot(
    x="species",
    y="petal_length",
    data=df,
    palette="rainbow"
    )

    
[vertopal.com_seaborn (2).pdf](https://github.com/user-attachments/files/25600901/vertopal.com_seaborn.2.pdf)

<img width="658" height="526" alt="image" src="https://github.com/user-attachments/assets/f9a7ace8-b9c8-47da-b8b5-9eec3e26b0cc" />


<img width="763" height="795" alt="Screenshot 2026-02-27 155510" src="https://github.com/user-attachments/assets/de4f24e3-5b38-44dc-a374-ebb845c09606" />

<img width="765" height="778" alt="Screenshot 2026-02-27 155457" src="https://github.com/user-attachments/assets/ec7202b5-4cd8-4b32-a253-0e3fa400ce43" />

<img width="761" height="718" alt="Screenshot 2026-02-27 155445" src="https://github.com/user-attachments/assets/728b58aa-a7a9-4a21-a786-698256eb5933" />

<img width="718" height="612" alt="Screenshot 2026-02-27 155418" src="https://github.com/user-attachments/assets/2cd11e84-8128-42d4-a056-0fd257095fcd" />

<img width="710" height="619" alt="Screenshot 2026-02-27 155404" src="https://github.com/user-attachments/assets/5c277ba7-04da-428a-9c9c-3a8c300f7c75" />

<img width="723" height="596" alt="Screenshot 2026-02-27 155349" src="https://github.com/user-attachments/assets/fe32736f-e6cb-460f-a9c1-e44c92115a4d" />

<img width="726" height="602" alt="Screenshot 2026-02-27 155338" src="https://github.com/user-attachments/assets/be706ec4-b08a-4515-bae0-db79565e4490" />

# Result:
successfully Performed Data Visualization using seaborn python library for the given datas
