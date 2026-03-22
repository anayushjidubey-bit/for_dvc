# --- Initial Setup ---
balance = 1000.00
pin = 1234
is_running = True

print("Welcome to Python Bank!")
entered_pin = int(input("Enter your 4-digit PIN: "))

# --- Simple Security Check ---
if entered_pin != pin:
    print("Wrong PIN. Access Denied.")
    is_running = False

# --- Main ATM Loop ---
while is_running:
    print("\n--- ATM MENU ---")
    print("1. Check Balance")
    print("2. Deposit Money")
    print("3. Withdraw Money")
    print("4. Exit")
    
    choice = input("Select an option (1-4): ")

    if choice == '1':
        print(f"Your current balance is: ${balance}")

    elif choice == '2':
        deposit_amount = float(input("Enter deposit amount: "))
        if deposit_amount > 0:
            balance += deposit_amount
            print(f"${deposit_amount} deposited successfully.")
        else:
            print("Invalid amount.")

    elif choice == '3':
        withdraw_amount = float(input("Enter withdrawal amount: "))
        if withdraw_amount > balance:
            print("Insufficient funds!")
        elif withdraw_amount <= 0:
            print("Invalid amount.")
        else:
            balance -= withdraw_amount
            print(f"${withdraw_amount} withdrawn successfully.")

    elif choice == '4':
        print("Thank you for using our ATM. Goodbye!")
        is_running = False
    
    else:
        print("Invalid choice, please try again.")