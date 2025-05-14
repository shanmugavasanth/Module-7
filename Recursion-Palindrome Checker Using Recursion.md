# 🔁 Recursion:Palindrome Checker Using Recursion in Python
## NAME : Shanmuga Vasanth M
## REG NO: 212223040191
## 🎯 AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

## 💻 PROGRAM:
~~~c
def is_palindrome(s):
    if len(s) <= 1:
        return True
    if s[0] == s[-1]:
        return is_palindrome(s[1:-1])
    else:
        return False
test_string = input("Enter a string: ").strip().lower().replace(" ", "")

if is_palindrome(test_string):
    print("The string is a palindrome.")
else:
    print("The string is not a palindrome.")
~~~

## OUTPUT
![442486408-d65bd6c5-861d-4ae2-9e14-ea292b599298](https://github.com/user-attachments/assets/0d117aca-28f8-41ea-8a4b-ee0c1a2c97da)


## RESULT
Thus,the program has been executed successfully.
