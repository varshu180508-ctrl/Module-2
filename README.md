# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a = 16
print(bin(a))
```
## Output
![442892759-23e036bf-9310-495e-8883-0a068b5cece1](https://github.com/user-attachments/assets/a9de7c63-6ec4-4612-aa8c-c12ec6e91e2f)

## Result
The program successfully converts the number 16 into its binary representation and prints it.

# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a, b):
    return a % b

a = int(input())
b = int(input())
print("The result of the modulo operation is:", result(a, b))
```
## Output
![442893816-1d6cd4c7-b1ce-42b7-87a8-054b1cc2b7f8](https://github.com/user-attachments/assets/73565b25-fa40-4cce-b63d-ca9a04fe24a6)
## Result
The program successfully defines a function that computes the modulo of two numbers and returns the result.

# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
i=int(input())
j=int(input())
z=int(input())
f = lambda a, b,c: a+b+c
print(f(i, j,z))
```
## Output
![442896655-df270927-b951-4377-9362-5ca11d0c2b69](https://github.com/user-attachments/assets/d94f9c73-b771-4625-b390-d3dff174da5c)

## Result
The program successfully defines a lambda function that computes the sum of two numbers and prints the result.

# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
rows = int(input())
coef = 1

for i in range(1, rows+1):
    for space in range(1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end = " ")
    print()
```
## Sample Output
![442896396-c9ed51f4-5c8a-45e4-9647-bf01f33923d7](https://github.com/user-attachments/assets/0c175e32-b4a4-4c3b-a8fe-0bdbef1e310a)

## Result
The program successfully generates Pascal's Triangle with the specified number of rows, using the appropriate formula for combination values.

## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input())
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print(f"{num} is a palindrome.")
else:
    print(f"{num} is not a palindrome.")
```
## Output
![442897869-68e6f75b-95cb-4c18-9b42-5e62186d34f4](https://github.com/user-attachments/assets/b25590d2-6c17-4707-8c4f-16b460e23df1)

## Result
The program successfully checks if a given number is a palindrome by reversing its digits and comparing it to the original number.
