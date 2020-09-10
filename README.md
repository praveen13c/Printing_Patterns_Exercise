# Printing_Patterns_Exercise
An exercise given by Harry to Print pattern on basis given input
# This is a Exercise given by Harry from Code with Harry Youtube Channel
# Coder = Praveen Singh Chauhan

# Program Starts

# Condition and comparison
while True:

    # all variables and inputs
    num01 = 1
    print("*" * 30)
    print("   Pattern Printing Exercise ")
    print("*" * 30)
    n = input("Enter A Number Please > ")

# stopping error to exit the programe
    try:
        n == int(n)
    except Exception as err_pp:
        print(f"Error = ", err_pp, "\n")
        continue

    n = int(n)
    b = input("Select Your preference & Enter [ 0 = True | 1 = False ] > ")

    try:
        b == int(b)
    except Exception as err_pp:
        print(f"Error = ", err_pp, "\n")
        continue

    if int(b) == 0:
        print(f" Your Number is '{n}' and its 'True'")

        while num01 != n + 1:
            print(num01, "*" * num01)
            num01 += 1
        else:
            print("Congratulations... Exercise is OVER ")
            break

    elif int(b) == 1:
        print(f" Your Number is '{n}'  and its 'False'")

        while n != 0:
            print(n, "*" * n)
            n -= 1
        else:
            print("Congratulations... Exercise is OVER ")
            break

    else:
        print("Enter [0] for 'True' or [1] for 'False' \n")
        continue

# Program Ends
