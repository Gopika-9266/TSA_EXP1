
### Name: Gopika R
### Register No: 212222240031
###  Date: 

# Ex.No: 01A PLOT A TIME SERIES DATA

## AIM:

To Develop a python program to Plot a time series data for Tesla Stock Predication.

## ALGORITHM:

1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Use pd.to_datetime to convert date/month/year to year.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.

   
## PROGRAM:

```
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('tsla_2014_2023 (1).csv')
data.head()
data["date"]=pd.to_datetime(data["date"])
plt.plot(data['date'], data['close'], label='Time Series Data')
plt.xlabel('Date')
plt.ylabel('Price')
plt.title('Time Series Plot')
plt.legend()
plt.show(block=False)
plt.show()
```


## OUTPUT:

![exp1 img](https://github.com/user-attachments/assets/c69ca8fb-0f18-452f-9954-f72621303795)


## RESULT:

Thus we have created the python code for plotting the time series of given data.
