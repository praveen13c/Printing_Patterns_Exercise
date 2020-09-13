# Printing_Patterns_Exercise
An exercise given by Harry to Print pattern on basis given input
# This is a Exercise given by Harry from Code with Harry Youtube Channel
# Coder = Praveen Singh Chauhan

# Program Starts

while True:  # Condition and comparison

    num01 = 1
    print("*" * 30)
    print("   Pattern Printing Exercise ")
    print("*" * 30)
    print("Enter 'exit' to end the program")
    n = input("Enter A Number Please (how many rows) > ")

    if str(n).lower() == "exit":
        print("OK... We are Exiting the Program >>>> ")
        break

    try:  # stopping error to exit the program
        str(n) == int(n)
    except Exception as err_pp:
        print("-" * 57)
        print(f"| Error = ", err_pp, "|")
        print("-" * 57, "\n")
        continue

    print("-> " * 20)
    n = int(n)
    n_both = n

    if n >= 10:  # Preventing to print more than 10 rows
        print(" please enter less than 10 ")
        continue

    b = input("Select Your preference & Enter [ 1 = Ascending | 0 = Descending | 2 = Both  ] > ")

    try:   # stopping error to exit the program
        b == int(b)
    except Exception as err_pp:
        print("-" * 57)
        print(f"| Error = ", err_pp, "|")
        print("-" * 57, "\n")
        continue

    b1 = int(b)
    b_b = bool(b1)
    print("-> " * 20)

    if b1 ==2:  # Printing both patterns one by one
        while n != 0:
            print(n, "*" * n)
            n -= 1
        print("")
        if n == 0:
            while num01 != n_both + 1:
                print(num01, "*" * num01)
                num01 += 1
            num01 = 1

    elif b1 >2:
        print("Enter [0] for 'Ascending' or [1] for 'Descending  or [2] for 'Both' ' \n")
        continue

    elif b_b == True:
        print(f"Your Number is '{n}' and its '{b_b}'")
        print("Printing Ascending Patterns ")
        while num01 != n + 1:
            print(num01, "*" * num01)
            num01 += 1

    elif b_b == False:
        print(f"Your Number is '{n}'  and its '{b_b}'")
        print("Printing Descending Patterns ")
        while n != 0:
            print(n, "*" * n)
            n -= 1

    else:
        print("Enter [0] for 'True' or [1] for 'False' \n")
        continue

# Program Ends
