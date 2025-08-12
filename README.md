# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:




import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('tesla_2014_2023.csv')
data.head()
data["date"]=pd.to_datetime(data["date"])
plt.plot(data['date'], data['close'], label='Time Series Data')
plt.xlabel('Date')
plt.ylabel('Price')
plt.title('Time Series Plot')
plt.legend()
plt.show(block=False)
plt.show()






# OUTPUT:
<img width="831" height="566" alt="image" src="https://github.com/user-attachments/assets/3e7bd959-0eb7-43d1-b36d-38e879687ac4" />






# RESULT:
Thus we have created the python code for plotting the time series of given data.
