# py
# Fault Calculator
#This is a "Fault Python Calculator". It does simple mathematical(+,-,*,/) calculation with wrong answer for fixed input values.  
#Print wrong answers for 25*3=28, 5.5+5=60, 12/6=6

#Code Begins
result = None

operator = input("Enter a mathematical operator(+,-,*,/): ")
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

if operator == "+":
    result = num1 + num2
    if result == (5.5+5):
        result = 60.0

elif operator == "-":
    result = num1 - num2

elif operator == "*":
    result = num1 * num2
    if result == (25*3):
        result = 28.0

elif operator == "/":
    result = num1 / num2
    if result == (12/6):
        result = 6.0

print("\nThe result is...")
print(num1, operator, num2, "=", result)
