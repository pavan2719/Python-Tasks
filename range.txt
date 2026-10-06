# 1. sum of prime numbers

# for j in range (20,150):
#     count = 1
#     for i in range (2,j+1):
#         if j % i == 0:
#             count =count+1
#     if count == 2:
#         print(j)


# 2. average of perfect numbbers

# perfect_avg = 0
# count = 0
# perfect_sum = 0
# for j in range (1,1000):
#     sum = 0
#     for i in range (1,j):
#         if j % i == 0:
#             sum = sum +i
#     if sum == j:
#         perfect_sum += sum
#         count = count + 1
# perfect_avg = perfect_sum / count
# print(perfect_avg)



# 3. leap year

# for j in range(1900,2026+1):
#     if (j % 4 ==0 and j % 100 != 0) or (j % 400 ==0):
#         print(f'{j} is leap year')



# 4. palindrome numbers iin range of 100 and 500

# for j in range(100,500):
#     n = j
#     rev = 0
#     while n != 0:
#         rem = n % 10
#         rev = rev * 10 + rem
#         n = n // 10
#     if rev == j:
#         print(f'{j} is a palindrome numbber')


# 5. digit sum = 10

# for j in range(120,851):
#     n = j
#     rev = 0
#     while n != 0:
#         rem = n % 10
#         rev = rev + rem
#         n = n // 10
#     if rev == 10:
#         print(f'{j} is a digit  numbber')


# 6. pair sum taget

# for j in range(1,50):
#     for i in range(j,50):
#         if i + j == 30:
#             print(f'({j},{i})')


# 7. 3 factor

# for j in range(1,300):
#     count = 0
#     for i in range(1,j+1):
#         if j % i == 0:
#             count += 1
#     if count == 3:
#         print(f'{j} has perfect 3 factors')


# 8. pime factors

# for j in range(20,50):
#     count = 0
#     print(f'prime factors of {j}')
#     for i in range(1,j+1):
#         if j % i == 0:
#             k=2
#             count = 1
#             while k != i+1:
#                 if i % k == 0:
#                     count = count + 1
#                 k = k + 1
#             if count == 2:
#                 print(f'{i} ')


# 9. amstron numbbers in range of 100 to 999

# for j in range(100,1000):
#     am = 0        
#     n= j
#     while n !=0:
#         rem = n % 10
#         am = am + (rem * rem * rem)
#         n = n // 10
#     if am == j:
#         print(f"{j} is amstrong number")


# 10. maximum factors

# max = 0
# for j in range(50,150):
#     count = 0
#     for i in range (1,j+1):
#         if j % i == 0:
#             count = count + 1
#     if count > max:
#         max = count
#         num = j
# print(f'{num} has maximum factors')