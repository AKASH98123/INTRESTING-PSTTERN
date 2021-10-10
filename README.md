# INTRESTING-PSTTERN

n=int(input("ENTER THE NUMBER OF ROWS :"))
for i in range(n):
    for j in range(i+1):
        x=0
        for k in range(j):
            #This loop is not run when j=0 hence x still remain 0
            x=x+n-k
        if j%2==0:
            print(x+i+1-j,end=" ")
        else:
            print(x+n-i,end=" ")        
    print()
    
    ##########################################################
    
    
n=int(input("ENTER THE NUMBER OF ROWS :"))
for i in range(n):
    x=i+1
    for j in range(i+1):
        y=n-j-1
        print(x,end=" ")
        x=x+y
    print()


##################@############################################@@@#######################


n=int(input("ENTER THE NIUMBER OF ROWS "))
for i in range(n):
    k=i+1
    for j in range(n-i-1):
        print(" ",end="  ")
    for j in range(i+1):
        print(k,end=" ")
        k=k-1
    if i>0:
        for j in range(i-1):
            print(" ",end=" ")
        for j in range(i+1):
            k=k+1
            print(k,end=" ")
    print()
for i in range(1,n):
    k=n-i
    for j in range(1,i+1):
        print(" ",end="  ")
    for j in range(n-i):
        print(k,end=" ")
        k=k-1
    if i<(n-1):
        for j in range(n-i-2):
            print(" ",end=" ")
        for j in range(n-i):
            k=k+1
            print(k,end=" ")
    print()
    
    
    
    ####################################################################################
    
    
    n=int(input("ENTER THE NUMBER OF ROWS"))

for i in range(1,n+1):
    k=ord("a")+n-1
    x=ord("a")+n+1-i
    for j in range(1,n-i+1):
        print(end=" ")
    for j in range(1,i+1):
        print(chr(k),end="")
        k=k-1


    for j in range(2,i+1):
        print(chr(x),end="")
        x=x+1
    print()

for p in range(n-1,0,-1):
    k=ord("a")+n-1
    x=ord("a")+n+1-p
    for j in range(1,n-p+1):
        print(end=" ")
    for j in range(2,p+2):
        print(chr(k),end="")
        k=k-1
    for j in range(1,p):
        print(chr(x),end="")
        x=x+1
    print()            


##############################################################################################################


n=int(input("ENTER THE NUMBER OF ROWS "))
for i in range(1,n+1):
    for j in range(1,n+1):
        if j==1 or j==n or i==(n+1)/2:
            print("*",end="")
        else:
            print(end=" ")
    print()

for i in range(1,n+1):
    for j in range(1,n+1):
        if j==1 or i==1 or i==n or i==(n+1)/2:
            print("*",end="")
        else:
            print(end=" ") 
    print()           

for i in range(1,n+1):
    for j in range(1,n+1):
        if j==1 or i==n:
            print("*",end="")
        else:
            print(end=" ")
    print()

for i in range(1,n+1):
    for j in range(1,n+1):
        if j==1 or i==n:
            print("*",end="")
        else:
            print(end=" ")
    print()

for i in range(1,n+1):
    for j in range(1,n+1):
        if i==1 or i==n or j==1 or j==n:
            print("*",end="")
        else:
            print(end=" ")
    print()
                                
                                   
######################################################################################################



num=int(input("ENTER THE NUMBER OF ROWS "))
l1=[[0 for x in range(num)] for y in range(num)]
low=0
n=1
high=num-1
count=int((num+1)/2)
for i in range(count):
    for j in range(low,high+1):
        l1[low][j]=n
        n=n+1
    #print 1 to 5
    for j in range(low+1,high+1):
        l1[j][high]=n
        n=n+1
    #print 6 to 9
    for j in range(high-1,low-1,-1):
        l1[high][j]=n
        n=n+1
    #print 10 to 13
    for j in range(high-1,low,-1):
        l1[j][low]=n
        n=n+1
    #print 13 to 15
    low=low+1
    high=high-1

for i in range(num):
    for j in range(num):
        print(l1[i][j],end="\t")
    print()
