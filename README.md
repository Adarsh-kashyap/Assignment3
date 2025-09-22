# Assignment3
#Task 1: Calculate Factorial Using a Function

# Program to calculate factorial of a number using recursion

def factorial(n):
    """Recursive function to calculate factorial"""
    if n == 0 or n == 1:   # base case
        return 1
    else:
        return n * factorial(n - 1)  # recursive call

# Taking input from user
num = int(input("Enter a number: "))

# Checking for negative numbers
if num < 0:
    print("Factorial is not defined for negative numbers.")
else:
    print("The factorial of", num, "is:", factorial(num))



#Task 2: Using the Math Module for Calculations
# Program to calculate square root, natural log, and sine of a number

import math

# Taking user input
num = float(input("Enter a number: "))

# Validity check (sqrt and log need positive numbers)
if num <= 0:
    print("Square root and natural log are not defined for zero or negative numbers.")
else:
    # Calculations using math module
    sqrt_val = math.sqrt(num)       # Square root
    ln_val = math.log(num)          # Natural log (base e)
    sine_val = math.sin(num)        # Sine in radians

    # Display results
    print("Square root",":", sqrt_val)
    print("Logarithm", ":",  ln_val)
    print("Sine",":" ,  sine_val)
    
