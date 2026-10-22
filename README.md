# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input values
2. Import the required packages.
3. Code the program.
4. Print the output.

## Program:

### Program to find the solution of a matrix using Gaussian Elimination.
### Developed by: GOWTHAM K
### RegisterNumber: 26014578

### import os
### os.environ["OPENBLAS_NUM_THREADS"]="1"
### import numpy as np
### import sys
### n=int(input())
### a=np.zeros((n,n+1))
### x=np.zeros(n)
### for i in range(n):
###    for j in range(n+1):
###        a[i][j]=float(input())
### for i in range(n):
###    if a[i][j]==0.0:
###        sys.exit('Divide by zero detected!')
###    for j in range(i+1,n):
###        ratio = a[j][i]/a[i][i]
###        for k in range(n+1):
###            a[j][k]=a[j][k]-ratio*a[i][k]
### x[n-1]=a[n-1][n]/a[n-1][n-1]
### for i in range(n-2,-1,-1):
###    x[i]=a[i][n]
###    for j in range(i+1,n):
###        x[i]=x[i]-a[i][j]*x[j]
###    x[i]=x[i]/a[i][i]
### for i in range(n):
###    print('X%d = %0.2f'%(i,x[i]),end=' ')

## Output:
![gaussian elimination]()

<img width="1369" height="523" alt="Screenshot 2026-10-22 215609" src="https://github.com/user-attachments/assets/ab7dcb99-517f-47cd-9af8-95c7326a3309" />

<img width="1381" height="335" alt="Screenshot 2026-10-22 215655" src="https://github.com/user-attachments/assets/4851fe5f-c8c2-4227-8c08-4a6ab41f7cbe" />

<img width="1391" height="486" alt="Screenshot 2026-10-22 215717" src="https://github.com/user-attachments/assets/69116258-3aa4-4fbd-8985-c007481bfd37" />



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

