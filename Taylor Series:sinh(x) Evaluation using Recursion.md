# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
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
~~~c
power = 0
fact = 1
def sinh_series(x, n):
    global power, fact
    if n == 0:
        return 0
    result = sinh_series(x, n - 1)
    exponent = 2 * n - 1
    power = power * x * x if power != 0 else x 
    fact *= exponent * (exponent - 1) if fact != 1 else 1   
    return result + power / fact
x = float(input("Enter the value of x: "))
n = int(input("Enter the number of terms (n): "))
power = 0
fact = 1
result = sinh_series(x, n)
print(f"\nsinh({x}) using {n} terms is: {result:.5f}")
~~~

## OUTPUT
![442486931-35025ff5-d59e-4a2a-8af7-d16e56e379f5](https://github.com/user-attachments/assets/d318b28b-3fb6-4838-8c4c-859de25e1b54)


## RESULT
Thus the program has been executed successfully.
