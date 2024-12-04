# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the `lu` function from the `scipy.linalg` package.
2. Get input from the user and print the L and U matrices using the `print` function.
3. Import `lu_factor` and `lu_solve` from the `scipy.linalg` package and create a variable `X` to include these functions.
4. Print the variable `X` and end program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: S Rajath
RegisterNumber: 24900186
'''

import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U) 
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: S Rajath
RegisterNumber: 24900186
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
B = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv), B)
print(X)
```

## Output:
**For finding L and U matrix**

![Screenshot 2024-12-04 145516](https://github.com/user-attachments/assets/4164cd04-7019-4d72-ad27-e73ecdfd2c01)

**To solve a matrix**

![image](https://github.com/user-attachments/assets/bbe6b488-02bb-4221-9ddb-f801169b4844)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

