# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file


# CODE
import pandas as pd
df = pd.read_csv("Data_set.csv")
df.head(10)
df.tail()
df.info()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df.head(10)
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df.head()
df['rating']=df['rating'].fillna(df['rating'].mean())
df.info()
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df.info()
df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])
df.info()
[df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mode()[0])
df.info()
df['watchers']=df['watchers'].fillna(df['watchers'].mode()[0])
df.head()
df.info()
df.isnull().sum()
# OUPUT
![Screenshot (122)](https://user-images.githubusercontent.com/79370364/161581355-ad61d997-d2eb-46c6-b5a0-bf8c279e6be7.png)
![Screenshot (123)](https://user-images.githubusercontent.com/79370364/161581522-160a8466-7f61-46d1-b3e2-0b87f0c9436f.png)
![Screenshot (124)](https://user-images.githubusercontent.com/79370364/161581701-6316cd08-3e5e-4eb9-8e7e-49333deecc07.png)
![Screenshot (125)](https://user-images.githubusercontent.com/79370364/161582084-5753c7b7-a00c-48ec-bf1a-718d18b56128.png)
![Screenshot (126)](https://user-images.githubusercontent.com/79370364/161582303-0cbdee9c-8911-4890-bde9-3a93b6e1fe85.png)
![Screenshot (127)](https://user-images.githubusercontent.com/79370364/161582549-b973f1a6-43d8-443b-b4e8-bea3d6ee9c9a.png)

