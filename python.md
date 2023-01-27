# welcome to python

![RedHeartHeartGIF](https://user-images.githubusercontent.com/114099821/214374280-1009c440-a44a-43d2-96d5-ff07f773352e.gif)


### "Unlocking the Power of Python: A Beginner's Guide to Mastering the World's Most Popular Programming Language"

### In this blog, we are covering almost all we need to know, to start with python 👍

### Installtion of Python

#### Step : 1
Download version (3.11.1) https://www.python.org/downloads/

#### Step : 2
Go to below link and download the pycharm community version. It was user friendly and responsive provoded by Jetbrains to run python programs.

Download (windows / macos)
https://www.jetbrains.com/pycharm/download/#section=windows


                                                            We are all set to go...😉😍


### Let's get into introduction to python

> Python is one of the most popular programming languages in present era, and it is easy for beginners to learn because of its readability which alomost similar to english words.

> It is dynamically typed, so no need to provide the data types, it consists of both structure/procedural oriented and object-oriented programming.

> Python is Interpreted language, which interprets line by line. 


## Python Concepts Started.....😁


### Python Indentation
> Indentation refers to the tab-spaces at the beginning of a code line.

> Where in other programming languages like c, c++, Java we use curly braces {} as the block of code, but in python indentation acts as a block of code, indentation in Python is very important.


### Basic Example

1.1 code

    print("Hello World!)
    
    

### Data types
>since python was dynamically typed, we don't need to specify data types, python interpreter will understand those types at run time.

1.2 code
    
    # to declare int
    a = 5
    
    # to declare float
    a = 5.0
    
    # to declare String
    b = "python" or b = 'python'
    
    by the way! '#' refers to comments, which are used to make code more readable and understandable by end-users.
    
    
### Type Casting
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
    
    
## String Fucntions


### String slicing
> Returns the sub string from the original string, python has 2 slicing methods
### one is using the built-in slice() method and another using the [:] array slice.

### array slicing syntax

s = 'python'

s[starting index : Ending index (inclusive) : number of indices to move]

#### Example

1.4 code
    
    s = "Hello, World!"

    print(s[0:5])  # output, Hello  (0 th index to 5 th index)
    print(s[2:5])  # output, llo    (2 nd index to 5 th index)
    print(s[1:4])  # output, ell    (1 st index to 4 th index)


    print(s[0:len(b):2]) # output, Hlo ol!         (0 th index till the length of the string, with escapes every 2nd character)
    print(s[0:len(b)])   # output, Hello, World!   (0 th index till the length of the string)


### built-in slice() syntax

slice(start index, end index, step count)

start - Optional. An integer number specifying starting posiotion of slice. Default is 0

end - ending position of the slicing

step - is is alos and Optional feild. An integer number specifying the step of the slicing. 1 step is default

#### Example

1.5 code

    a = ["a", "b", "c", "d", "e"]
    x = slice(2)
    print(a[x]) # output, ['a', 'b', 'c']
    
    a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    x = slice(5, 8, 3)
    print(a[x]) # output, [6]



### Highly used string methods in problem solving.

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

### clear example

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
        
### Boolean

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
    
    
### Operators

> Operators was used to do some tasks on variables.

`Operators and Operands`

> Operators are symbols/signs and Operands are variables.

![operator-and-operands-2-1504587480626](https://user-images.githubusercontent.com/114099821/214359830-ecb29f88-5e18-4733-8001-1c4b57c52df2.png)


## Some important operators

> Arithmetic operators
> 
> Assignment operators
> 
> Comparison operators
> 
> Logical operators
> 
> Bitwise operators

### Arithmetic operators
> These are the simple mathematical operators.

> It consists of : "+", "-", "*", "/", "%", "//"

1.8 code
    
    a = 5
    b = 5

    print (a + b) # output, 10
    print (a - b) # output, 0
    print (a * b) # output, 25
    print (a / b) # output, 1
    print (a % b) # output, 0. This is modulos operator
    print (a //b) # output, 1. This is Floor Division, used to avoid floating points, and output was always an int type();
    
### Assignment operators
> Used to assign values to variables

1.9 code

    a = 5
    a += 3 or a = a + 3 (both are same)
    print(a) # output, 8

    a = 5
    a -= 3 or a = a - 3
    print(a) # output, 2

    a = 5
    a *= 3 or a = a * 3
    print(a) # output, 15

    a = 5
    a /= 3 or a = a / 3
    print(a) # output, 1.666

    a = 5
    a //= 3 or a = a // 3
    print(a) # output, 1

### Comparison operators
> Comparison operators are used to compare two values

> True or False, this is the output for every comparision

2.0 code
    
    a = 5
    b = 5

    print (a == b) # output, True
    print (a != b) # output, False
    print (a > b)  # output, False
    print (a < b)  # output, False
    print (a >= b) # output, True
    print (a <= b) # output, True

### Logical opretors

> Basially it do some logical operations, and returns either True or False.

> logical and : returns True if and only if both the conditons are true.
> logical or : returns True if any of the conditon is true.
> logical not : it reverse the answer.

2.1 code
    
    a = 5
    print(a > 3 and a < 10)
    # returns True because both conditions are correct.

    a = 5
    print(a > 10 or a < 10)
    # returns True because one of the conditions are correct.


    x = 5
    print(not (x > 10 or x < 10))
    # general answer was True.
    # but returns False, because not is used to reverse the answer.
    
### Bitwise operators

> It works with a binary numbers.

It contains the following;

> & (AND)

> | (OR)

> ^ (XOR)

> ~ (NOT)

`we deep dive into bitwise operators in further topics (bit-manipulation)`


## Conditions and If-else Statements
 
> As the name suggests, if else statements work based on the condition.


#### what is condition ?

> The expression which was included in the if () part is said to be condition, it may be anything like mathematical expression, logic for your code etc.


#### what is statement ?

> followed by if and else conditions, these are the actions that we need to do, when the condition was True or False

> If condition is True, then the block of code present inside the if or the if - statements was executed. otherwise else part comes into action. 

### if () and else() example 

2.2 code
    
    age = 20
    
    if (age >= 18):
        print("Eligible for license")
    else:
        print("Not Eligible for license")
        
    # output, "Eligible for license"
    Explanation : age >= 18 this condition satisfies the given input.
        

### elif (else if) 😶‍🌫️😶‍🌫️

> just like if() this is another checking condition, if your code having many checking conditions we use elif() ! as simple it is.

2.3 code

    temperatue = 24
    
    if (temperatue > 30):
        print("Too hot !!!")

    elif (temperatue < 15):
        print("Too cold !!!")
        
    else:
        print("Moderate")
        
    # output, "Moderate"


## Loops (Control Statements)
> As the name itself defines, we can control the execution of loops

#### What is a Loop ??

When we want to execute our code multiple times then we place our code in a loop
Basically a loop is also based on if - condition, The code inside it only executes when the condition is met True.
We have 2 Types of loops:
> for and 
> while


## for - Loop
> We use this loop when we know how many times our block of code needs to be executed...

#### Syntax
   > for i in range(starting_index, ending_index(inclusive), step_value)


   > for i in range(n):     (here i starts from 0,, i gets incremented by 1 every time after the block of code under it executes,, condition is i < n)


   > for i in range(1,n,2): (here i starts from 1,, i gets incremented by 2 every time after the block of code under it executes.. condition is i < n)
 
2.4 code

    a = 0
    for i in range(5):
        a += i   # a = a + i
    print(a)

    # Output:
        10
 
## while - Loop

> We use this loop when we want our block of code to get executed till the condition is met False.

> Make sure that the condition is met False in future, since there is a chance of loop getting stuck to infinity
### (cause, love you for infinity..♾️💚).

> The reason is, we know that the while loops run until the conditions holds True, so if there is no False condition the loops runs for infinite times.

#### Syntax


    while (condition == True):

      // Group of statements
      // increment/decrement
  
  > Example
  
      n = 5
      while (i < n):
          print(i)
          i = i + 1
          
      (here loop executes till the condition (i < n) met False)
 
2.5 code
  
    a = 0
    while(a < 5):
        a += 1    # a = a + 1
        print(a)
     
    # Output:
        1
        2
        3
        4
        5


# Lists (Data Structures or what 🫡🤨)

> Lists are used to store multiple items in a single variable, when you are working with large data, we can store the data in the lists.

> It Provides various functionalites.

> to create a list use [] brackets or list().

### These are the complete properties of list.

![p](https://user-images.githubusercontent.com/114099821/215129878-602df074-0585-4b3a-bfe9-d2c8af86e9a5.png)


## Syntax 

## mylist = [] or mylist = list()

#### we access the list elements using index, the index starts from 0, and to get length of list use --> len(mylist)

2.6 code
   
## Accessing list elements by using index.
   
    mylist = [1, 2, 3, 4, 5]

    print(mylist[0])  # output, 1

    print(mylist[2])  # output, 3
   
## using for loop to print list items.
   
   
     mylist = ["BMW", "Rolce Roice", "Ferrari"]

     for i in range(len(mylist)):

        print(mylist[i])
       
    # output :

    BMW
    Rolce Roice
    Ferrari
      
   
   
   
   
