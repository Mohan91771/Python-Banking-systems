class Banking:
    def __init__(self,balance):
        self.__balance=balance
        print(f"You Avaliable Balance is {balance}.")

    def Card(self,pin,name):
        self.pin=pin
        self.name=name

    @staticmethod
    def greet():
        print("Insert your card")
        print("=========================")

    def Number(self,num):
        self.num=num
        while num < 20 or num > 99:
            print("Invalid number")
            print("Select 20 to 99 numbers")
            m=int(input("Enter number:"))
            break
        print("=========================")
        
    def withdraw(self,action):
        if action == "withdraw":
            n=int(input("Enter amount to withdraw:"))
            while n>self.__balance:
                print("Insufficient funds. Try again.")
                n=int(input("Re-Enter Amount:"))
            pins=int(input("Enter your pin:"))
            while pins != self.pin:
                pins=int(input("Re-Enter pin:"))
            self.__balance -= n
            print("Withdrawal successful.")
            print("===========================")
            show_balance = input("Do you want to see your balance? (yes/no): ").strip().lower()
            if show_balance == "yes":
                print(f"Your balance: ${self.__balance}")
                print("===========================")
                print("Thank you!")
            else:
                print("===========================")
                print("Thank You!")
                    
    def deposit(self, action):
        if action =="deposit":
            amount=int(input("Enter Amount: "))
            pins = int(input("Enter PIN: "))
            while pins != self.pin:
                pins = int(input("Re-Enter PIN: "))
            self.__balance += amount
            print("Deposit successful.")
            print("===========================")
            show_balance = input("Do you want to see your balance? (yes/no): ").strip().lower()
            if show_balance == "yes":
                print(f"Your balance: ${self.__balance}")
                print("===========================")
                print("Thank you!")
            else:
                print("===========================")
                print("Thank You!")
            
    def balance(self):
        print(f"Your current balance is: ${self.__balance}.")
    @staticmethod
    def greets():
        print("Take Your Card!,Have A Nice Day.")




account=Banking(1000)
a=int(input("Set Your Pin upto 4 Digits:"))
b=input("Enter name:")
account.Card(a,b)
Banking.greet()
c=int(input("enter number 20 to 99 only:"))
account.Number(c)
action = input("Enter action(Withdraw/Deposit/Balance):").strip().lower()
if action in ["withdraw","deposit","balance"]:
    if action=="withdraw":
        account.withdraw(action)
    elif action=="deposit":
        account.deposit(action)
    else:
        account.balance()
Banking.greets()
