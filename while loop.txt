#1.Find the sum of digits in a given number.
n=738
sum=0
new=n
while n!=0:
    ld=n%10
    sum=sum+ld
    n=n//10
print(f"sum of digits {new} is = {sum}")

#2.Find the average of digits in a given number.
n=624
new=n
sum=0
count=0
while n!=0:
    ld=n%10
    sum=sum+ld
    count=count+1
    n=n//10
avg=sum/count
print(f"avg of digits {new} is = {avg}")

#3.Find the sum of the first digit and the last digit of a given number.
n=936
ld=n%10
while n>=10:
    n=n//10
first=n
print(f"first and last digit sum is {ld+first}")

#4.Find the average of digits that are divisible by 5 in a given number.
n=int(input("enter the number:"))
sum=0
count=0
while n>0:
    ld=n%10
    if(ld%5==0):
        sum=sum+ld
        count=count+1
    n=n//10
avg=sum/count
print(f"Average of digits that divisible by 5 is ={avg}")


#5.Find the difference between the largest digit and the smallest digit in a given number.
n=int(input("Enter the number:"))
diff=0
lar=0
small=9
while n!=0:
    ld=n%10
    if(ld>lar):
        lar=ld
    if(ld<small):
        small=ld
    n=n//10    
print("largest=",lar)
print("smallest =",small)
print(f"the difference detween the largest and smallest digit is = {lar-small}")