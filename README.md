### Developed By: KARTHIKEYAN R
### Register NO : 212222240046
### Date:
# Ex.No: 01A PLOT A TIME SERIES DATA
# AIM:
To Develop a python program to Plot a time series data (Date/Gold Price).
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Convert 'Date' column to datetime.
4. Plot 'Price' against 'Date'
5. Display the final gold price graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_csv("/content/Gold Price.csv")

# Convert the 'Date' column to datetime
data['Date'] = pd.to_datetime(data['Date'])

# Plotting the 'Price' column over time
plt.figure(figsize=(10,6))
plt.plot(data['Date'], data['Price'], label='Gold Price', color='gold')

# Adding title and labels
plt.title('Gold Price Over Time')
plt.xlabel('Date')
plt.ylabel('Price (INR)')

# Displaying the plot
plt.legend()
plt.grid(True)
plt.show()

```
# OUTPUT:
![EX-01A](https://github.com/user-attachments/assets/50799f42-fee2-4a07-969b-e012d8125bf5)


# RESULT:
Thus,the Python code has been created to visualize the time series of the given data.
