# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
# Univariate Linear Regression without libraries
# y = m*x + c



# Step 1: Calculate means
n = len(x)
mean_x = sum(x) / n
mean_y = sum(y) / n

# Step 2: Calculate slope (m) and intercept (c)
numerator = sum([(x[i] - mean_x) * (y[i] - mean_y) for i in range(n)])
denominator = sum([(x[i] - mean_x) ** 2 for i in range(n)])
m = numerator / denominator
c = mean_y - m * mean_x

# Step 3: Predict values
y_pred = [m * xi + c for xi in x]

# Step 4: Print results
print("Slope (m):", m)
print("Intercept (c):", c)
print("Predicted values:", y_pred)







```
## Output
</br> x = [1, 2, 3, 4, 5]
y = [2, 4, 5, 4, 5]

</br> Slope (m): 0.6
Intercept (c): 2.2
Predicted values: [2.8, 3.4, 4.0, 4.6, 5.2]


</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
