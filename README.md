# asg_3
# Exercise 1
months = ["January", "February", "March", "April", "May", "June",
              "July", "August", "September", "October", "November", "December"]

month_number = int(input("Enter the month (1-12): "))
if 1 <= month_number <= 12:
        print(f"Month {month_number} is {months[month_number - 1]}")
else:
        print("Error: Enter a number between 1 and 12.")


# Exercise 2

full_price = 6.0
age = int(input("Enter your age: "))

if age < 16:
    ticket_price = full_price / 2
elif age >= 60:
    ticket_price = full_price / 3
else:
    ticket_price = full_price
print(f"Your ticket costs £{ticket_price:.2f}")

# Exercise 3

weight = float(input("Enter your weight in (kg): "))
height = float(input("Enter your height in (m): "))
bmi = weight / (height ** 2)
if bmi < 18.5:
    category = "underweight"
elif 18.5 <= bmi <= 24.9:
    category = "normal"
elif 25 <= bmi <= 29.9:
    category = "overweight"
else:
    category = "obese"
print(f"Your BMI is: {bmi:.2f}")
print(f"You are in the \"{category}\" range.")

# Exercise 4

num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
num3 = float(input("Enter the third number: "))
if num1 >= num2 and num1 >= num3:
    greatest = num1
elif num2 >= num1 and num2 >= num3:
    greatest = num2
else:
    greatest = num3
print(f"The greatest number is: {greatest}")


# Exercise 5

num = int(input("Enter a non-negative integer: "))
if num < 0:
    print("Factorial is not defined for negative numbers.")
factorial = 1
for i in range(1, num + 1):
    factorial *= i
print(f"The factorial of {num} is: {factorial}")

# Exercise 6

num = int(input("Enter a number: "))

reversed_num = 0
original_num = num
while num > 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num //= 10
print(f"The reverse of {original_num} is: {reversed_num}")

# Exercise 7

num = int(input("Enter a number: "))
limit = int(input("Enter the range limit: "))
print(f"Multiples of {num} up to {limit}:")
for i in range(1, limit + 1):
    multiple = num * i
    if multiple > limit:
        break
    print(multiple)

# Exercise 8

while True:
    value = input("Please enter something (type 'done' to exit): ")
    if value.lower() == 'done':
        print("Done")
        break
    print(value)

# Exercise 9

for i in range(1, 11):
    if i % 3 == 0 and i % 5 == 0:
        print("FizzBuzz")
    elif i % 3 == 0:
        print("Fizz")
    elif i % 5 == 0:
        print("Buzz")
    else:
        print(i)

# Exercise 10

for i in range(5, 0, -1):
    for j in range(i, 0, -1):
        print(j, end=" ")
    print()
