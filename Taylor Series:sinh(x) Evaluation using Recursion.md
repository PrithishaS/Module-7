# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:

# Reg.No: 212222210020
# Name: Prithisha S

def fact(n):
    if n == 0:
        return 1
    return n * fact(n - 1)

def sinh(x, n):
    if n == 0:
        return x
    return sinh(x, n - 1) + (x**(2*n+1)) / fact(2*n+1)

x = int(input("Enter x: "))
n = int(input("Enter terms: "))

print("sinh(x):", sinh(x, n))

## OUTPUT

Enter x: 1
Enter terms: 3
sinh(x): 1.1752011936438014

## RESULT

The programs were implemented successfully and the outputs were verified.
