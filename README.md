import random
a=int(input("enter the starting range:"))
b=int(input("enter the ending range:"))
num=random.randint(a,b)
if(num%2)==0:
    print("{0} is a even number".format(num))
else:
    print("{0} is a odd number".format(num))
if num>0:
    print("{0} is a positive number".format(num))
else:
    print("{0} is a negative number".format(num))
if num>1:
    for i in range(2,num):
        if(num%i)==0:
            print(num,"is a composite number")
            break
    else:
            print(num,"is a prime number")
elif num==0 or 1:
        print(num,"is a neither prime nor composite number")
else:
        print(num,"is not a prime nor it is a composite number")
