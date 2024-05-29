# -Bank-Transaction-Management-system
The Bank Transaction Management System is a beginner-friendly project designed to introduce you to the basics of Python programming. This project simulates a simple banking system where users can manage their financial transactions. The main features include: 1. Deposit Funds: 2. Withdraw Funds: 3. Balance Inquiry: 4. Transaction History:

class account:
    def __init__(self,balance,acc_no):
        self.balance=balance
        self.acc_no=acc_no
    def debit(self,ammount):
        self.balance-=ammount
        print("Rs",ammount,"was debited")
        print("your account number is=",self.acc_no)
        print("your current balance is=",self.print_info())
    def credit(self,ammount):
        self.balance+=ammount
        print("Rs",ammount,"was credited")
        print("your account number is=",self.acc_no)
        print("your current balance is=",self.print_info())
    def print_info(self):
        return self.balance
s1=account(8000,12345)
s1.debit(1000)
s1.credit(5000)
