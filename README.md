# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
# Algorithm for program 1:
1. Read the square matrix 𝐴.
2. Use lu(A) from scipy.linalg to compute matrices 𝑃,𝐿,𝑈.
3. Store the lower and upper triangular matrices.
4. Print matrices L and U.
# Algorithm fro program 2:
1. Read coefficient matrix A and constant matrix B.
2. Apply lu_factor(A) to get LU decomposition and pivot info.
3. Use lu_solve() to solve AX=B using LU and pivot.
4. Print the solution vector X.


## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: N V Chetan Satwik
RegisterNumber: 212224240100
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.

Developed by: N V Chetan Satwik
RegisterNumber: 212224240100
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```

## Output:
<img width="1175" height="447" alt="image" src="https://github.com/user-attachments/assets/779b9d52-fb50-4b2a-87e7-2fd21a681154" />


<img width="859" height="186" alt="image" src="https://github.com/user-attachments/assets/94a9acd6-7c44-4848-b6cd-74c5c9532980" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

