
def menu():
    print("---Welcome to the banking.---")
    print("1. To check the balance.")
    print("2. To Deposit the amount. ")
    print("3. To withdraw the amount.")
    print("4. Quit.")

balance = 1000

while True:
    choice = int(input("Enter the choice:"))

    if choice == 1:
        print("Balance:",balance)
    elif choice == 2:
        amount = int(input("Enter the amount to be deposited:"))
        balance += amount
        print("The balance after deposite is:",amount)
    elif choice == 3:
        amount = int(input("Enter The amount to be withdrawn:"))
        
        if balance < amount:
            
            print("Insufficiant balance.")
        else:
            balance -= amount
            print(balance)
            
        
       
        
    elif choice == 4:
        print("Thanks for choosing us..")
        break
    else:
        print("Try again")
