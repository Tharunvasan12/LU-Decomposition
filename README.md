# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. The user is prompted to enter a matrix in the form of a nested list

2. The lu function performs LU decomposition with partial pivoting. P. Permutation matrix (to reorder rows for numerical stability). J. Lower triangular matrix (with ones on the diagonal). U Upper triangular matrix.

3. The Land U matrices are printed to the console

4. End of the program (ii) To find the LU Decomposition of a matrix

5. A square matrix representing coefficients of the linear equations. A column vector representing the right-hand side of the equations.

6. LU Factorization: lu_factor(A) performs an LU decomposition with partial pivoting, returning: piv: A pivoting information array. 3.Solving Ax=b. lu_solve((lu, piv), b) solves the equation efficiently using the LU decomposition. 4.End of the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by:Tharunish vasan.T
RegisterNumber:24001333 
*/
```
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Tharunish vasan.T
RegisterNumber:24001333 
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
![image](https://github.com/user-attachments/assets/d217dd2f-d1fa-43eb-8534-37f36306b7be)


![image](https://github.com/user-attachments/assets/8d8a672c-38f8-45df-ad9b-619fe7b06b02)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

