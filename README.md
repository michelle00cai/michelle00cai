# michelle00cai
Simple-Calculator-Python (3/28/20)
print("Select operation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")
choice = input("Enter choice(1/2/3/4): ")
choices = ["1", "2", "3", "4"]
if choice not in choices:
    print("cannot read, please pick 1,2,3 or 4")
else:
    input1 = input("Enter first number: ")
    try:
        num1 = float(input1)
    except ValueError:
        print("Input must be a number")
    input2 = input("Enter second number: ")
    try:
        num2 = float(input2)
        if choice == "1":
            print("The answer is " + str(num1 + num2))
        elif choice == "2":
            print("The answer is " + str(num1 - num2))
        elif choice == "3":
            print("The answer is " + str(num1 * num2))
        else:
            print("The answer is " + str(num1/num2))
    except ValueError:
        print("Input must be a number")
