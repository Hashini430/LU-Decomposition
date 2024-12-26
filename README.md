# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm01
1.Input the matrix:
  Read a matrix A from the user input.
2.Perform LU Decomposition:
  Call the LU decomposition function (lu(matrix)) to get the L (lower triangular) and U (upper triangular) matrices.
3.Extract matrices:
  The lu() function returns three outputs:
  The permutation matrix P (which is not required for this task).
  The lower triangular matrix L.
  The upper triangular matrix U.
4.Display matrices:
  Output the L matrix (lower triangular matrix).
  Output the U matrix (upper triangular matrix).
```
## Algorithm02
1.Input the Matrix and the Vector:
  Read the matrix of size nxn and the vector b of nx1
  The matrix A represents the system of linear equations.
  The vector b contains the constants on the right-hand side of the equations.
2.LU Decomposition:
  Perform LU decomposition of the matrix A to obtain two matrices:
  L (lower triangular matrix)
  U (upper triangular matrix)
  This decomposition can be achieved using the lu_factor function from scipy.linalg.
3.Solve the System:
  Use the LU decomposition to solve the system of linear equations Ax=b.
  This is done using the lu_solve function, which uses the previously computed LU matrices to find the solution vector x.
4.Output the Solution:
  Print the solution vector x, which represents the solution to the system of linear equations.
  

## Program:
(i) To find the L and U matrix
```
/*
Program to find L and U matrix using LU decomposition.
Developed by: HASHINI R
RegisterNumber: 24900728

import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to solve a matrix using LU decomposition.
Developed by: HASHINI R
RegisterNumber: 24900728

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
b=np.array(eval(input()))
x=lu_factor(matrix)
solution=lu_solve(x,b)
print(solution)

*/
```

## Output:
![lu decomposition]()
![Alt text](<Screenshot from 2024-12-08 13-28-38.png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

