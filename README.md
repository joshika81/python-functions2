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
