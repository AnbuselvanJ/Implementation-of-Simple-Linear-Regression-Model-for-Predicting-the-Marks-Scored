# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
# Program to implement Simple Linear Regression
# for predicting the marks scored by a student

# Import required libraries
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Create the dataset directly
# Hours Studied vs Marks Scored
data = pd.DataFrame({
    'Hours': [1, 2, 3, 4, 5],
    'Marks': [35, 40, 50, 55, 60]
})

# Independent variable (X) and Dependent variable (y)
X = data[['Hours']]     # 2D input
y = data['Marks']

# Create the Linear Regression model
model = LinearRegression()

# Train the model
model.fit(X, y)

# Predict marks
predicted_marks = model.predict(X)

# Display slope and intercept
print("Slope (m):", model.coef_[0])
print("Intercept (c):", model.intercept_)

# Plot the data and regression line
plt.scatter(X, y, label="Actual Marks")
plt.plot(X, predicted_marks, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression for Predicting Marks")
plt.legend()
plt.show()
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by:Anbuselvan J 
RegisterNumber:212225230015  
*/
```

## Output:
![WhatsApp Image 2026-01-27 at 9 42 32 AM](https://github.com/user-attachments/assets/37713798-26f8-432b-a2b0-8f4874b5c525)


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
