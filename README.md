# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
i)To Find the L and U Matrix
Step 1:
Import NumPy and the lu function from SciPy to perform LU decomposition.

Step 2:
Take the input matrix from the user and convert it into a NumPy array A.

Step 3:
Use lu(A) to decompose the matrix into P (Permutation matrix), L (Lower triangular matrix), and U (Upper triangular matrix).

Step 4:
Print the L matrix and U matrix.


ii)To Find the LU Decomposition Solution of a Matrix

Step 1:
Import NumPy and lu_factor, lu_solve from SciPy to solve linear equations using LU decomposition.

Step 2:
Take input matrices A (coefficient matrix) and B (constant matrix) from the user.

Step 3:
Use lu_factor(A) to factorize matrix A, then use lu_solve() to find the solution matrix X.

Step 4:
Print the solution matrix X.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: 
RegisterNumber: 
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input())) 
lu,pivot=lu_factor(A)
X=lu_solve((lu,pivot),B)
print(X)
```

## Output:
(i) To find the L and U matrix
<img width="592" height="361" alt="EXP-5A" src="https://github.com/user-attachments/assets/08845b8f-3b0d-4da6-bf26-a54b3e45e138" />

(ii) To find the LU Decomposition of a matrix
<img width="592" height="184" alt="EXP-5B" src="https://github.com/user-attachments/assets/ca2c33f4-8c0e-45f2-8784-d6a46ac60665" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

