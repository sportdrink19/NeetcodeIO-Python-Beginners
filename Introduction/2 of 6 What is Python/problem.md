This course will teach you the core concepts of Python. But if you're a beginner, the most important thing you will learn is how to think like a programmer.

## Challenge
You can click the Submit button to execute the code on the right. Don't worry if you don't understand any of it.

You will notice that the output is incorrect. We want to calculate the first 20 digits of pi, but right now our program is only printing the first 19 digits. With the power of programming we can fix this by changing a single line of code.

To fix this, find the following line of code:

n = 19
and change the number to 20. Then click the Submit button again.

Hint: If you don't want to read through the code, click the editor and press Ctrl + F. You can then type "n = 19" to find the line of code you need to change.

## Starting code
```python
from decimal import Decimal, getcontext

def calculate_pi(n):
    getcontext().prec = n + 2  # Set precision higher than needed for accuracy
    
    C = 426880 * Decimal(10005).sqrt()
    K = 6
    M = 1
    X = 1
    L = 13591409
    S = L
    
    for i in range(1, n):
        M = (K ** 3 - 16 * K) * M // i ** 3
        L += 545140134
        X *= -262537412640768000
        S += Decimal(M * L) / X
        K += 12
    
    pi = C / S
    return str(pi)[:n + 2]  # Return first n digits plus the '3.'

n = 19
pi_digits = calculate_pi(n)
print(pi_digits)
```