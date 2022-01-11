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
    
