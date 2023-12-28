# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
## Step1:
Import the necessary libraries and get input from the user
## Step2: 
Use nested loops to iterate over each element of the matrix
## Step3:
Perform Gaussian elimination to solve the system of linear equations
## Step4:
Use back Substitution and Print the output
## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: MOHAMED AAKIF ASRAR S
RegisterNumber: 23003613
import numpy as np
n=int(input())
arr=np.zeros((n,n+1))
res=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
res[n-1]            =arr[n-1][n]/arr[n-1][n-1]
for i in range(n-1,-1,-1):
    res[i]=arr[i][n]
    for j in range(i+1,n):
        res[i]=res[i]-arr[i][j]*res[j]
    res[i]=res[i]/arr[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,res[i]),end=" ")
*/
```

## Output:
![Screenshot 2023-12-28 185704](https://github.com/MOHAMEDAAKIFASRAR/Gaussian/assets/148514683/512f50bd-f6e0-45e5-960c-8ac66149d081)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

