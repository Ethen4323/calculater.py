# calculater.py
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error: Cannot divide by zero!"

def power(x, y):
    return x ** y

def square (x):
    return x * x

def average(x, y, z):
    return (x + y + z) / 3

# Main program
print("Welcome to Function-based Calculator!")

while True:
    print("\nOptions:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Power")
    print("6. square")
    print("7. average")
    print("8. Exit")

    choice = input("Enter choice (1-8): ")

    if choice == "8":
        print("Exiting... Goodbye!")
        break

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: ")) if choice != "6" else 1
    num3 = float(input("Enter third number: ")) if choice == "7" else None


    if choice == "1":
        print("Result:", add(num1, num2))
    elif choice == "2":
        print("Result:", subtract(num1, num2))
    elif choice == "3":
        print("Result:", multiply(num1, num2))
    elif choice == "4":
        print("Result:", divide(num1, num2))
    elif choice == "5":
        print("Result:", power(num1, num2))
    elif choice == "6":
        print("Result:", square(num1))
    elif choice == "7":
        print("Result:", average(num1, num2 , num3))

    else:
        print("Invalid choice, please try again.")
# This code is a simple calculator that performs basic arithmetic operations.
