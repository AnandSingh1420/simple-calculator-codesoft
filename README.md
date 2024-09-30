# simple-calculator-codesoft

def addition(a,b):
    return a+b

def subtraction (a,b):
    return a-b

def multiplication (a,b):
    return a*b

def division (a,b):
    if b==0:
        return "Number can't be divided by 0"
    else:
        return a/b
    
print ("Select the operation--->")
print("Choose 1 for addition:")
print("Choose 2 for subtraction:")
print("Choose 3 for multiplication:")
print("Choose 4 for division:")

while True:
    operation= input ("ENTER THE OPERATION NUMBER YOU WANT TO PERFORM:")

    if operation in ('1','2','3','4'):
        n1= float(input("Enter first number:"))
        n2= float(input ("Enter second number:"))

        if operation == '1':
            print (n1, "+", n2, "=", addition(n1,n2))

        elif operation =='2':
            print (n1, "-",  n2, "=", subtraction(n1,n2))

        elif operation== '3':
            print (n1, "*", n2, "=", multiplication(n1,n2))

        elif operation== '4':
            print (n1, "/", n2, "=", division(n1,n2))

        next_calculation = input("Want to peform another calculation? (yes/no):")
        if next_calculation.lower()!= "yes":
            break
    else:
        print ("Invalid input")
