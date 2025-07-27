rint("CALCULATOR...!!!")
while True:
    try:
        num = int(input("Enter 1st number: "))
    except ValueError:
        print("Please enter a valid integer.")
        continue
    
    while True:
        opp = input("Enter operation (+, -, *, /): ")
        if opp in ["+", "-", "*", "/"]:
            break
        else:
            print("Please enter (+, -, *, /)...!!")
    
    try:
        num2 = int(input("Enter 2nd number: "))
    except ValueError:
        print("Please enter a valid integer.")
        continue

    if opp == "+":
        print(f"Result: {num + num2}")
    elif opp == "-":
        print(f"Result: {num - num2}")
    elif opp == "*":
        print(f"Result: {num * num2}")
    elif opp == "/":
        if num2 == 0:
            print("Error: Division by zero!")
        else:
            print(f"Result: {num / num2}")

    print('THANK YOU...!!')
