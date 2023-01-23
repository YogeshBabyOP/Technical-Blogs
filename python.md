## Python 

> Python is one of the most popular programming languages in present era, and it is easy for beginners to learn because of its readability which alomost similar to enligh words.

> It is dynamically typed, so no need to provide the data types, it consists of both structure/procedural oriented and object-oriented programming.

> Python is Interpreted language, which interprets line by line. 

#### Python Indentation
> Indentation refers to the tab-spaces at the beginning of a code line.

> Where in other programming languages like c, c++, Java we use curly braces {} as the block of code, but in python indentation acts as a block of code, indentation in Python is very important.


#### Basic Example

1.1 code

    print("Hello World!)
    
    
### Installtion of Python

#### Step : 1
Download version (3.11.1) https://www.python.org/downloads/

#### Step : 2
Go to below link and download the pycharm community version. It was user friendly and responsive provoded by Jetbrains to run python programs.

Download (windows / macos)
https://www.jetbrains.com/pycharm/download/#section=windows


                                                    We are all set to go...😉😉

#### Data types
>since python was dynamically typed, we don't need to specify data types, python interpreter will understand those types at run time.

1.2 code
    
    # to declare int
    a = 5
    
    # to declare float
    a = 5.0
    
    # to declare String
    b = "python" or b = 'python'
    
    by the way! '#' refers to comments, which are used to make code more readable and understandable by end-users.
    
    
#### Type Casting
> which means, changing the data types of a variable like int -> float, float -> int, int -> string etc.

1.3 code
    
    # converting int --> float
    x = 5
    x = float(x)
    print(x) # output will be 5.0
    
    # converting float --> int
    x = 12.5
    x = int(x)
    print(x) # output will be 12, it removes the floating points
    
    # converting String --> int
    x = "123"
    x = int(x)
    print(x) # output will be 123, now it is integer type, we can use as a number
    
    # converting int to string 
    x = 123
    x = str(x)
    print(x) # output will be "123", in terminal is doesn't show quotes, now we can perform all the string functions to x
