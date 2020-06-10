# step-numbers-from-1-to-N
a=int(input("enter num:"));p=0
for i in range(10,a+1):
    d,c=i,0
    while d>9:
        if abs(d%10-(d//10)%10)!=1:
            c=1
            break
        d//=10;
    if c==0:print(i,end=' ');p=1
if p==0:print(-1)
        
