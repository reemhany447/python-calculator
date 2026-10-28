# python-calculator
A simple Python calculator that takes two numbers and an operation (+, -, *, /), then prints the result. Uses match/case, and shows "Invalid" for division by zero or an unknown operation.

a = float(input("Enter first number: "))
b = float(input("Enter second number: "))
operation = input("Enter operation (+, -, *, /): ")

match (operation, b):
    case ("+", _):
        print(a + b)
    case ("-", _):
        print(a - b)
    case ("*", _):
        print(a * b)
    case ("/", 0):
        print("Invalid")
    case ("/", _):
        print(a / b)
    case _:
        print("Invalid")
