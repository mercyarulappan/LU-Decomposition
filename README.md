# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1.Read the elements of augmented matrix into arrays a and b
2.Calculate elements of L and U
3.Print elements of L and U
4.Find V by solving LV = B by forward substitution
5.Find X by solving UX = V by backward substitution
6.Print Array X as the solution

## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: Mercy A 
RegisterNumber: 212223110027
'''
from scipy.linalg import lu
a=eval(input())
P,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''Program to solve a matrix using LU decomposition.
Developed by: Mercy A
RegisterNumber: 212223110027
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=eval(input())
b=eval(input())
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:

![image](https://github.com/mercyarulappan/LU-Decomposition/assets/149233730/2d06ad71-021c-4ade-b230-93fb170ac0ac)

![image](https://github.com/mercyarulappan/LU-Decomposition/assets/149233730/c79d3cff-1dc6-49ea-8df4-57a59222cf0f)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

