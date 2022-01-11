# Banking.py
Banking basic application

import sys
class CUSTOMER:
 ''' Customer class with bank related operations'''
 bankname="IndusInd"
 
 def __init__(self,name,balance=0):
    self.name=name
    self.balance=0
    
 def Deposit(self.amt):
    self.balance=self.balance+amt
    print("After Deposit the balance is:",self.balance)
 def Withdraw(self,amt):
    if amt>self.balance:
      sys.exit()
    else:
      self.balance=self.balance-amt
      print("After withdrawl the balance is",self.balance)
 
 print("Welcome to:",CUSTOMER.bankname)
 name=input("Enter your name")
 c=CUSTOMER
 
 While True:
   print('d-deposit\nw-withdraw\ne-exit)
   option=input("Choose your Option")
   if option=='d' or option=='D':
    amt=float(input("Enter the amount to deposit:"))
    c.deposit(amt)
   elif option=='w' or option=='W':
    amt=float(input("Enter the amount to Withdraw:"))
    c.withdraw(amt)
   elif option=='e' or option=='E':
    print('Thanks for Banking')
    sys.exit()
   else:
    print("Choose a valid option")
