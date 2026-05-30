# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Here is the algorithm for the Python program you provided to find the inverse of a matrix using NumPy.

---

### **Algorithm: Matrix Inversion Using NumPy**

#### **Step 1: Start**

The execution of the program begins.

#### **Step 2: Environment Configuration (Optional optimization)**

Set the environment variable `OPENBLAS_NUM_THREADS` to `"1"`. This limits the OpenBLAS library to a single thread, preventing CPU over-allocation during linear algebra operations.

#### **Step 3: Import Necessary Libraries**

* Import the `os` module to interact with the operating system environment.
* Import the `numpy` library as `np` to handle multi-dimensional arrays and matrix operations.

#### **Step 4: Define the Matrix**

Initialize a $3 \times 3$ square matrix using `np.array()`.


$$\text{matrix} = \begin{bmatrix} 1 & 0 & 3 \\ -1 & 2 & -2 \\ 2 & 3 & -1 \end{bmatrix}$$

#### **Step 5: Compute the Inverse**

Call the built-in function `np.linalg.inv()` and pass the defined matrix as the argument.

> **Note:** This function calculates the multiplicative inverse of a square matrix. Mathematically, it solves for $A^{-1}$ such that $A \cdot A^{-1} = I$, where $I$ is the identity matrix.

#### **Step 6: Store the Result**

Assign the computed inverse matrix to the variable named `result`.

#### **Step 7: Display Output**

Print the calculated inverse matrix (`result`) to the console.

#### **Step 8: Stop**

The program terminates successfully.

## Program:
#Program to find the inverse of a matrix.
#Developed by:R.JAYETHAN
#RegisterNumber:212225240057
import os
os.environ["OPENBLAS_NUM_THREADS"]= "1"
import numpy as np
matrix=np.array([[1,0,3],[-1,2,-2],[2,3,-1]])
result= np.linalg.inv(matrix)
print(result)
## Output:
<img width="1918" height="980" alt="Screenshot 2026-04-29 094111" src="https://github.com/user-attachments/assets/b58ecd45-ebd5-41ab-accf-78283a162522" />

## Result:
Thus the inverse of given matrix is successfully solved using python program

