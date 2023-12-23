# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the elements of augmented matrix into array A and B
2. Calculate elements of L and U
3. Print L and U matrix
4. Find V  by solving LV=B by forword substitution
5. Find X by solving UX=V by backward substitution
6. Print array X as the solution
## Program:
(i) To find the L and U matrix
```python
Program to find the L and U matrix.
Developed by: VASANTHARAJ J
RegisterNumber: 23012935
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
Program to find the LU Decomposition of a matrix.
Developed by: VASANTHARAJ J
RegisterNumber: 23012935
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A,B=eval(input()),eval(input())
lu,piv=lu_factor(A)
x = lu_solve((lu,piv),B)
print(x)
```
## Output:
(i) To find the L and U matrix.
![image](https://github.com/Vasanth2k4/LU-Decomposition/assets/147139769/0ef13be4-02e4-47ea-a5c2-6cc80c74ae30)

(ii) To find the LU Decomposition of a matrix.
![image](https://github.com/Vasanth2k4/LU-Decomposition/assets/147139769/93a11784-068d-4570-a0a0-4236614ed2d7)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

