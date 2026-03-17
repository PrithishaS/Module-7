# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:

# Reg.No: 212222210020
# Name: Prithisha S

def head_recursion(n):
    if n == 0:
        return
    head_recursion(n - 1)
    print(n)

n = int(input("Enter number: "))
head_recursion(n)

## OUTPUT

1
2
3
4
5

## RESULT

The programs were implemented successfully and the outputs were verified.
