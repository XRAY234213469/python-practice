# python-practice
Python practise tasks
**Name**: Mutua Wilson Mwendwa 
**Admission Number**: 184179
## Tasks
This repository contains my solutions to Python practice tasks, including writing custom functions for sum, even/odd checking, factorials, string reversal, and sum of digits.
python-practice/
│
├── README.md
├── sum_list.py
├── check_even_odd.py
├── factorial_loop.py
├── reverse_string.py
├── factorial_recursive.py
└── sum_of_digits.py
# Function to sum all elements in a list
# Thought Process: Iterate through the list, add each element to a total

def sum_list(numbers):
    total = 0
    for num in numbers:
        total += num
    return total

# Example usage
print(sum_list([1, 2, 3, 4, 5]))  # Output: 15
# Function to check if a number is even or odd
# Thought Process: Use modulo operator %

def check_even_odd(number):
    if number % 2 == 0:
        return "Even"
    else:
        return "Odd"

# Example usage
print(check_even_odd(7))  # Output: Odd
# Function to compute factorial using a loop
# Thought Process: Multiply numbers from 1 to n

def factorial_loop(n):
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

# Example usage
print(factorial_loop(5))  # Output: 120
# Function to reverse a string without slicing or built-in methods
# Thought Process: Loop through the string backwards manually

def reverse_string(s):
    reversed_s = ""
    for char in s:
        reversed_s = char + reversed_s
    return reversed_s

# Example usage
print(reverse_string("hello"))  # Output: "olleh"
# Function to compute factorial recursively
# Thought Process: Base case n==0 or n==1, otherwise n * factorial(n-1)

def factorial_recursive(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial_recursive(n - 1)

# Example usage
print(factorial_recursive(5))  # Output: 120
# Function to compute sum of digits
# Thought Process: Extract each digit using modulo and integer division

def sum_of_digits(number):
    total = 0
    while number > 0:
        digit = number % 10
        total += digit
        number //= 10
    return total

# Example usage
print(sum_of_digits(1234))  # Output: 10

