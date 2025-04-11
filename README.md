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
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt


data = pd.read_csv("/content/daily-minimum-temperatures-in-me.csv")

x = data.iloc[:, 0]  
y = data.iloc[:, 1]  


plt.figure(figsize=(10, 5))
plt.xlabel("Date")
plt.ylabel("Minimum Temperature (°C)")
plt.title("Daily Minimum Temperatures Over Time")
plt.plot(x, y, linestyle='-', color='blue')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
[[]]
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/e535db9b-896f-4764-a442-534ae769c818)





# RESULT:
Thus we have created the python code for plotting the time series of given data.
