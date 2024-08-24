# Ex.No: 01A PLOT A TIME SERIES DATA

### Developed by : M.Pranathi
### Register No : 212222240064
###  Date: 


# AIM:
To Develop a python program to Plot a time series data of Supermarket sales.


# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Plot the data according to need and can be altered monthly, or yearly.
4. Display the graph.


# PROGRAM:

```
import pandas as pd
import matplotlib.pyplot as plt
df=pd.read_csv('supermarketsales.csv')
df.head()

df['Date'] = pd.to_datetime(df['Date'])
plt.figure(figsize=(10, 6))
plt.bar(df['Date'], df['Total'])
plt.title('Dialy Total Sales')
plt.xlabel('Date')
plt.ylabel('Total Sales')
plt.xticks(rotation=45)
plt.show()
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/06f287ae-da73-42a5-b201-449b25aa9fad)


![image](https://github.com/user-attachments/assets/e9c53026-180f-4dc8-96d4-a7e45a86d712)

# RESULT:
Thus we have created the python code for plotting the time series of given data.
