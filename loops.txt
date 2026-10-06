# Average of numbers from 1 to N
n = int(input("Enter N: "))
sum = 0
for i in range(1, n + 1, 1):
    sum = sum + i
average = sum / n
print("Average:", average)

# Sum of squares from 1 to N
n = int(input("Enter N: "))
sum = 0
for i in range(1, n + 1, 1):
    sum = sum + i * i
print("Sum of squares:", sum)

# Sum of cubes from 1 to N
n = int(input("Enter N: "))
sum = 0
for i in range(1, n + 1, 1):
    sum = sum + i ** 3
print("Sum of cubes:", sum)

# Calculate power without using **
base = int(input("Enter base: "))
power = int(input("Enter power: "))
result = 1
for i in range(1, power + 1, 1):
    result = result * base
print("Result:", result)

# First N terms of Fibonacci series
n = int(input("Enter N: "))
a = 0
b = 1
for i in range(1, n + 1, 1):
    print(a)
    c = a + b
    a = b
    b = c

# Series 1, 1/2, 1/3, 1/4, ...
n = int(input("Enter N: "))
for i in range(1, n + 1, 1):
    print(1 / i)

#Series 1, 11, 111, 1111, ...
n = int(input("Enter N: "))
num = 0
for i in range(1, n + 1, 1):
    num = num * 10 + 1
    print(num)

#Series 1, 3, 9, 27, 81, ...
n = int(input("Enter N: "))
num = 1
for i in range(1, n + 1, 1):
    print(num)
    num = num * 3