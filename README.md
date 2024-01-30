# Codsoft_1
#calculator.py 
def calculator():
    while True:
        print("\nOperations: \n1. Addition (+)\n2. Subtraction (-)\n3. Multiplication (*)\n4. Division (/)\n5. Exit")
        choice = input("Enter the number of the operation you want to perform: ")
        if choice in ('1', '2', '3', '4', '5'):
            if choice == '5':
                break
            num1 = float(input("Enter the first number: "))
            num2 = float(input("Enter the second number: "))
            if choice == '1':
                print(f"Result: {num1 + num2}")
            elif choice == '2':
                print(f"Result: {num1 - num2}")
            elif choice == '3':
                print(f"Result: {num1 * num2}")
                print(f"Result: {num1 * num2}")
            elif choice == '4':
                if num2 == 0:
                    print("Error: Division by zero is not allowed.")
                else:
                    print(f"Result: {num1 / num2}")
        else:
            print("Invalid input. Please enter a number between 1 and 5.")

calculator()
