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
```
def fun(n):
if (n >0):
fun(n - 2)
print(n-1,
end=" ) x =
int(input())
if(x%2==0):
fun(x )
 else:
fun(x+1)
```

## OUTPUT
<img width="458" height="148" alt="image" src="https://github.com/user-attachments/assets/c3a3965d-df0f-40f8-82c2-2a617555f6da" />

## RESULT
Thus, the given program is implemented and executed successfully.

# 🔁 Recursion:Palindrome Checker Using Recursion in Python

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
```
def is_palindrome(word): if
len(word)<1:
return True
else:
if word[0]==word[-1]:
return is_palindrome(word[1:-1]) else:
return False word
= str(input())
Saveetha Engineering College
if is_palindrome(word)==True: print("String
is a palindrome")
else:
print("String is not a palindrome")
```

## OUTPUT
<img width="436" height="214" alt="image" src="https://github.com/user-attachments/assets/27f30702-4023-482e-a0ca-76f8952ab93c" />

## RESULT
Thus, the given program is implemented and executed successfully .

# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
```
def sum_of_digits(n):
 # Base case: if n is 0, return 0
 if n == 0:
 return 0
 else:
 # Recursive case: last digit + sum of remaining digits
 return n % 10 + sum_of_digits(n // 10)
# Input from the user
number = int(input())
# Handling negative numbers
number = abs(number)
```

## OUTPUT
<img width="229" height="148" alt="image" src="https://github.com/user-attachments/assets/8cdf3209-f87a-4803-970f-c438c25abcd0" />

## RESULT
Thus the program has been successfully executed.

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
```
def series(x,n):
if n==0:
return
1 else:
return
x**n/n+series(x,n-1) x =
int(input())
n =
int(input())
print(series(x))
```

## OUTPUT
<img width="351" height="162" alt="image" src="https://github.com/user-attachments/assets/f513d315-1acd-4071-bd92-cd1704aacef8" />

## RESULT
Thus, the given program is implemented and executed successfully.

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
```
def fact(n):
if n<=1:
return 1
else:
return n*fact(n-1)
def sinh(x,n):
if n==0:
return x
else:
return (pow(x,(2*n+1))/fact(2*n+1))+sinh(x,n-1)
x=int(input())
n=int(input())
print(sinh(x,n))
```

## OUTPUT
<img width="507" height="114" alt="image" src="https://github.com/user-attachments/assets/98a937da-6b9f-476b-a583-d82c475c12ab" />

## RESULT
Thus the program has been successfully executed.
