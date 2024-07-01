# 1. Calculate the Area of a Rectangle:

length = 5
width = 3
area = length * width
print(f"The area of the rectangle is: {area}")

# Output:
# The area of the rectangle is: 15

# 2. Check if a Number is Even or Odd:

numb = 6
if numb % 2 == 0:
    print("number is even")
else:
    print("number is odd")
    
# output:
# 6 is odd.

# 3. Reverse a String:

# Reverse a String
strs = input("Enter a strs: ")
reverse_strs = strs[::-1]
print("Reversed string",reverse_strs)

# Output:
 # Reversed string: olleH

 # 4. Find the Factorial of a Number

def factorial(num):
    if num == 0:
        return 1
    else:
        return num * factorial(num-1)

numb = 5
rslt = factorial(numb)
print(f"Factorial of {numb} is: {rslt}")

 # 5. Check if a String is Palindrome or Not

strs = radar
if strs == strs[::-1]:
    print(strs,"is a palindrome.")
else:
    print( strs, " is not a palindrome.")
# Output:
# radar is a palindrome.


# 6. Generate Fibonacci Series up to n terms

    def fibonacci(number):
    if number == 1:
        return [0]

    a = 0
    b = 1
    fibo = [0, 1]

    for i in range(2, number):
        n = a + b
        a = b
        b = n
            
        fibo.append(n)
        
    return fibo


num_input = int(input("Enter the number of terms : "))

print(f"Fibonacci Series up to {num_input} terms : {fibonacci(num_input)}")
# Output:
# Fibonacci Series up to 6 terms: 0, 1, 1, 2, 3, 5

# 7. Find the Largest Among Three Numbers

numbers = list(map(int, input("Enter three numbers separated by space: ").split()))
largest_number = max(numbers)
print("The largest number is:", largest_number)

# Output:
# The largest number is: 25


# 8. Calculate Simple Interest

principal = float(input("Enter the principal amount: "))
rate = float(input("Enter the rate of interest: "))
time = float(input("Enter the time period in years: "))
simple_interest = (principal * rate * time) / 100
print("Simple Interest:", simple_interest )

# Output:
# Simple Interest: 100.0

# 9. Convert Celsius to Fahrenheit

celsius = float(input("Enter temperature in Celsius: "))
fahrenheit = (celsius * 9/5) + 32
print("Temperature in Fahrenheit:",fahrenheit)

# Output:
# Temperature in Fahrenheit: 98.6

# 10. Check Leap Year

year = int(input("Enter a year: "))
if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print(year," is a leap year.")
else:
    print(year,"is not a leap year.")
    
# Output:
# 2024 is a leap year.


# Programming Challenges
# 1. Find the Median of Three Numbers

def find_median():
    numbers = list(map(int, input("Enter three numbers separated by space: ").split()))
    numbers.sort()
    if len(numbers) % 2 == 0:
        median = (numbers[len(numbers)//2 - 1] + numbers[len(numbers)//2]) / 2
    else:
        median = numbers[len(numbers)//2]
    print(f"Median is: {median}")

find_median()

# Output:
# Median is: 10

# 2. Count the Number of Words in a Sentence

sentence = input("Enter a sentence: ")
words = sentence.split()
print("Number of words:",len(words))

# Output:
# Number of words: 9


# 3. Calculate the Sum of Digits in a Number

def calculate_sum_of_digits():
    number = input("Enter a number: ")
    sum_of_digits = sum(int(digit) for digit in number)
    print("Sum of digits:", sum_of_digits)

calculate_sum_of_digits()

# Output:
# Sum of digits: 15

# 4. Find the Longest Common Prefix in a List of Strings

def longest_common_prefix(strs):
    if not strs:
        return ""
    shortest_str = min(strs, key=len)
    for i, char in enumerate(shortest_str):
        for other in strs:
            if other[i] != char:
                return shortest_str[:i]
    return shortest_str

def main():
    strings = input("Enter strings separated by space: ").split()
    prefix = longest_common_prefix(strings)
    print(f"Longest common prefix: {prefix}")

if __name__ == "__main__":
    main()


# Output:
# Longest common prefix: fl

# 5. Check if a Number is a Prime Number

def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

number = int(input("Enter a number: "))
if is_prime(number):
    print(number, "is a prime number.")
else:
    print(number, "is not a prime number.


# Output:
# 29 is a prime number.







