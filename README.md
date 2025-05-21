# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) 
1.Start

2.Read the input matrix A.

3.Call the LU decomposition function: P, L, U = lu(A)

P is the permutation matrix (used internally)

L is the lower triangular matrix

U is the upper triangular matrix

Print the matrices L and U.

4.End 
(ii) 
1.Start

2.Read the coefficient matrix A and the right-hand side vector b.

3.Compute LU decomposition using: lu, piv = lu_factor(A)

lu contains the combined LU matrix

piv stores pivoting information

Solve the system using: x = lu_solve((lu, piv), b)

Print the solution vector x.

4.End

## Program:
(i) To find the L and U matrix

```Program to find the L and U matrix.

Developed by:Mohana K.V.S.L
RegisterNumber:24900659
```
import numpy as np

from scipy.linalg import lu

A = np.array(eval(input()))

P,L,U = lu(A)

print(L)

print(U)

(ii) To find the LU Decomposition of a matrix
```Program to find the LU Decomposition of a matrix.
Developed by:Mohana K.V.S.L
RegisterNumber:24900659
```
# To print X matrix (solution to the equations)

import numpy as np

from scipy.linalg import lu_factor, lu_solve

a = np.array(eval(input()))

b = np.array(eval(input()))

lu, piv = lu_factor(a)

x = lu_solve((lu, piv), b)

print(x)


## Output:
(i)L and U matrix
![Screenshot 2025-05-16 195238](https://github.com/user-attachments/assets/3c2bb788-4e64-45ec-9fa3-51f67a29bdbe)

(ii)LU Decomposition of a matrix
![Screenshot 2025-05-16 195251](https://github.com/user-attachments/assets/93ceee96-efc9-46ca-8b83-00cea9a9322e)






## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

