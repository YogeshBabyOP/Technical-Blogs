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
    
    
### String Fucntions


##### String slicing
> Returns the sub string from the original string, python has 2 slicing methods
> one is using the in-build slice() method and another using the [:] array slice.

`array slicing syntax`

s = 'python'

s[starting index : Ending index (inclusive) : number of indices to move]

`Example`

1.4 code
    
    s = "Hello, World!"

    print(s[0:5])  # output, Hello  (0 th index to 5 th index)
    print(s[2:5])  # output, llo    (2 nd index to 5 th index)
    print(s[1:4])  # output, ell    (1 st index to 4 th index)


    print(s[0:len(b):2]) # output, Hlo ol!         (0 th index till the length of the string, with escapes every 2nd character)
    print(s[0:len(b)])   # output, Hello, World!   (0 th index till the length of the string)


`built-in slice() syntax`

slice(start index, end index, step count)

start	Optional. An integer number specifying starting posiotion of slice. Default is 0

end	    ending position of the slicing

step	is is alos and Optional feild. An integer number specifying the step of the slicing. 1 step is default

`Example`

1.5 code

    a = ["a", "b", "c", "d", "e"]
    x = slice(2)
    print(a[x]) # output, ['a', 'b', 'c']
    
    a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    x = slice(5, 8, 3)
    print(a[x]) # output, [6]



#### Highly used string methods in problem solving.

>.upper()

 converts the string to upper case

>.lower()

 converts the string to lower case
 
>.count()

 counts for a specific string
 
>.split(" ")

 split the string with commas and empty spaces

>.strip()

 removes leading white spaces
 
>.replace()

 replaces the mentioned character in the string
 
>.concat() or use + for concatination

 concates or combines two or more strings together
 
>.capitalize()

 makes first letter of a text or string to Capital

>.title()

 make all the first letter of every word to capital

1.6 code

        a = "Hello, World!"
        print(a.upper())
        # output, HELLO, WORLD!

        a = "Hello, World!"
        print(a.lower())
        # output, hello, world!
        
        a = "12345"
        print(a.count("1"))
        # output, 1 (as only one  '1' is present)
        
        a = "Hello, World!"
        b = a.split(",")
        print(b)
        # output, ['Hello', ' World!']

        a = "     Hello, World!     "
        print(a.strip())
        # output, Hello, World!


        a = "Hello, World!"
        print(a.replace("H", "J"))
        # output, Jello, world!

        a = "Hello"
        b = "World"
        print(a + b)
        # output, helloWorld

        s = "hello, welcome to yogesh's git."
        x = s.capitalize()
        print (x)
        # output, Hello, welcome to yogesh's git.


        s = "hello, welcome to yogesh's git."
        x = s.title()
        print(x)
        # output, Hello, Welcome To Yogesh'S Git.
        
#### Boolean

Similar to other programming languages boolean represents two things True or False.
we can evaluate any expression to know whether it's True or False;

`Example`

1.7 code

    a = 5
    b = 3
    print(a > b) # output, True
    
    a = 5
    b = 3
    print(b > a) # output, False
    
    
    In python, there is a built-in method bool(), to find it's nature.
    
    a = 5
    print(bool(a)) # output, True
    
    a = 0
    print(bool(a)) # output, False
    
    a = 1
    print(bool(a)) # output, True
    
    > Since in computer therory, 1 refers to True and 0 refers to False.
    
    s = ""
    print(bool(s)) # output, False (Empty string also False, notice s = "" != s = " ")
    
    
    
