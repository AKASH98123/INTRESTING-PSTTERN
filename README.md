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
                                   
            
