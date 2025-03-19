# Intro to Python Assignment

**Activity:** Basic Calculator Program
- Create a simple Python program that asks the user to input two numbers and a mathematical operation (addition, subtraction, multiplication, or division).
- Perform the operation based on the user's input and print the result.
- *Example:* If a user inputs 10, 5, and +, your program should display 10 + 5 = 15.

**Solution:**
```
def calculator():
    print("Welcome to the Basic Calculator Program! 🧮")
    print("--------------------------------------------")

    # Store the first and second number from the user
    num1 = float(input("\nEnter the first number: "))
    num2 = float(input("\nEnter the second number: "))

    # Store the operation from the user
    operation = input("\nEnter the operation (+, -, *, /): ")

    # Calculate the result based on the operation
    if operation == "+":
        result = num1 + num2
        print(f"Solution: {num1} + {num2} = {result}")
    elif operation == "-":
        result = num1 - num2
        print(f"Solution: {num1} - {num2} = {result}")
    elif operation == "*":
        result = num1 * num2
        print(f"Solution: {num1} * {num2} = {result}")
    elif operation == "/":
        if num2 == 0:
            print("Sorry: Cannot divide by zero!")
        else:
            result = num1 / num2
            print(f"Solution: {num1} / {num2} = {result}")
    else:
        print("\nInvalid operation! Please enter a valid operation +, -, *, /.")
    
    print("\n--------------------------------------------")
    print("Thanks for using the Basic Calculator Program! 😊")

# Run the program
calculator()
```
