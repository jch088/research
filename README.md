# research

# Python program to display all the prime numbers within an interval

lower = 900
upper = 1000

print("Prime numbers between", lower, "and", upper, "are:")

for num in range(lower, upper + 1):
# all prime numbers are greater than 1
if num > 1:
for i in range(2, num):
if (num % i) ==0:
break

else:
print(num)

# Python program to find factorial of a number provided

# change the value for a different result
num = 7

# To take input from user
#num = int(input("Enter a number: '))

factorial = 1

# check if the number is negative, positive or zero
if num < 0:
print("Sorry, factorial does not exist for negative numbers")
elif num == 0:
print("The factorial of 0 is 1")
else:
for i in range(1,num + 1):
factorial = factorial*i
print("The factorial of",num,"is",factorial)

# Find the LCM of two input numbers

def compute_lcm(x,y):

# choose the greater number
if x > y:
greater = x
else:
greater = y

while(True):
if((greater % x == 0) and (greater % y == 0)):
lcm = greater
break
greater += 1

return 1cm

num1 = 54
num2 = 24

print("The L.C.M. is", compute_lcm(num1, num2))


# Calculate power of a number using a while loop

base = 3
exponent = 4

result = 1

while exponent != 0:
result *= base
exponent-=1

print("Answer = " + str(result))
