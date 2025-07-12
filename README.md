#functions within functions:
def outer():
    print("This is the outer function.......")
    def inner():
        print("This is the inner function........")
    inner()
outer()
............output..............
This is the outer function.......
This is the inner function........



def cal(a,b):
    def add():
        return a+b
    def sub():
        return a-b
    def mul():
        return a*b
    def div():
        return a/b
    print("addition", add())
    print("subtraction", sub())
    print("multiplication", mul())
    print("division", div())
a=int(input("enter a number:"))
b=int(input("enter a number:"))
cal(a,b)
............output..............
enter a number: 4
enter a number: 5
addition 9
subtraction -1
multiplication 20 
division 0.6666666666666666



def mul_by(n):
    def inner(x):
        return x*n
    return inner
times_2=mul_by(2)
times_3=mul_by(3)
print(times_2(5))
print(times_3(10))
............output..............
10
30
