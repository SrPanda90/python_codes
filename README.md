# python_codes
It comprises some simple problems and its solution codes.

""" QUESTION: Array of integers are given we have to return indices of two numbers 
              such that they add up to specifc target (TARGET IS THE SUM)
"""


print("........PROGRAM STARTED.........")

n=int(input("How many numbers do you want to Enter: "))
arry=[]

for i in range(n):
    s=int(input(F"ENter nummber {i+1}:"))
    arry.append(s)

target=int(input("ENter  target sum:"))

for i in range(n):    
    for j in range(-1,-n,-1):
        ct=True
        if(arry[i]+arry[j]==target):
            ct=False
            print(f"Indexes are:{arry.index(arry[i])},{arry.index(arry[j])}")
    
if (ct== True):
    print("No index found.")
    
print(".........SUCCESSFULLY IMPLEMENTED.........")
