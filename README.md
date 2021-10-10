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
            
