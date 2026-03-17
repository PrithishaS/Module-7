# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:

# Reg.No: 212222210020
# Name: Prithisha S

def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

def taylor(x, n):
    if n == 0:
        return 1
    return taylor(x, n - 1) + (x**n) / factorial(n)

x = int(input("Enter x: "))
n = int(input("Enter terms: "))

print("Taylor Series:", taylor(x, n))

## OUTPUT

Enter x: 1
Enter terms: 5
Taylor Series: 2.708333333333333

## RESULT

The programs were implemented successfully and the outputs were verified.
