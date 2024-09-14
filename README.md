Implementation of Univariate Linear Regression
AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

Equipments Required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook
Algorithm
Get the independent variable X and dependent variable Y.
Calculate the mean of the X -values and the mean of the Y -values.
Find the slope m of the line of best fit using the formula.
image

4. Compute the y -intercept of the line by using the formula:
image

5. Use the slope m and the y -intercept to form the equation of the line. 6. Obtain the straight line equation Y=mX+b and plot the scatterplot.
Program:
karthikeyan
212223040088

import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='blue')
plt.plot(X,Y_pred,color='yellow') 
plt.show() 
Output:
output output

Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming

