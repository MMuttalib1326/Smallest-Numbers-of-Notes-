# Smallest-Numbers-of-Notes-
Consider a currency system in which there are notes of six denominations, namely, Rs. 1, Rs. 2, Rs. 5, Rs. 10, Rs. 50, Rs. 100. If the sum of Rs. N is input, write a program to computer smallest number of notes that will combine to give Rs. N.


t=int(input())
for i in range(t):
    N=int(input())
    l=[100,50,10,5,2,1]
    c=0
    for i in l:
        if(N>=i):
            c+=N//i
            N=N%i
    print(c)
