# 📐 Taylor Series Using Recursion in Python
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
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
~~~c
power = 1
fact = 1
def taylor_series(x, n):
    global power, fact

    if n == 0:
        return 1
    result = taylor_series(x, n - 1)
    power *= x
    fact *= n
    return result + (power / fact)
x = float(input("Enter the value of x: "))
n = int(input("Enter the number of terms (n): "))
result = taylor_series(x, n)
print(f"\nThe value of e^{x} using Taylor series (n={n} terms) is: {result:.5f}")
~~~

## OUTPUT
![442486706-5bd2a165-53c6-448e-8297-2774f150dd10](https://github.com/user-attachments/assets/2ea419c6-e758-4322-aa3c-a80fcde208cc)


## RESULT
Thus the program has been executed successfully.
