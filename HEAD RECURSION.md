# 🔁 Types of Recursion: Head Recursion in Python
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
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
~~~c
def sum_of_digits(n):
    return sum(int(digit) for digit in str(abs(n)))
def head_recursive_sequence(n):
    if n <= 0:
        return
    digit_sum = sum_of_digits(n)
    if digit_sum % 2 == 0:
        head_recursive_sequence(n - 1)
    else:
        head_recursive_sequence(n - 2)
    print(n, end=' ')
number = 10
print(f"Head Recursive Sequence starting from {number}:")
head_recursive_sequence(number)
~~~

## OUTPUT
![442486230-f45c9121-34d9-4b67-bfe4-ad16b6443e75](https://github.com/user-attachments/assets/fd2e699f-2e0e-4e69-b3bf-a5920361a486)


## RESULT
Thus the program has been executed successfully.
