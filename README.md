# 20.max-and-min-prime-from-a-list
l=[]
k=[]
n=int(input('Enter how many numbers you want in a list:'))
for i in range(n):
      l.append(int(input('Enter the number:')))     
for i in l:
    c=0
    for j in range(1,i+1):
        if i%j==0:
            c=c+1  
    if c==2:
        k.append(i)
print('Maximum Prime Number is',max(k))
print('Minimum Prime Number is',min(k))
