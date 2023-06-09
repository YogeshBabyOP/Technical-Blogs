# This blog contains all of my learning about Php servers and its usage in the Backend. 💀☠️ 
<br>

## Let's Get Started... 🏎️🏎️🏎️

<br>

### Print statement in Php.

    <?php
        echo "Hello God!";  // output : Hello God!
    ?>

<br>

### Variables in Php. <br>
> The syntax is quite similar to javaScript template literals. 

    <?php

        $name = "Lucifer"; // string
        $age = 1000;      // int
        $GPA = 10.0;     // float
        $god = true;    // boolean

        echo "My name is {$name}, like the devil !<br>";  // output :  My name is Lucifer, like the devil !
        echo "I'm {$age} years old <br>";                // output : I'm 1000 years old
        echo "My gpa is {$GPA} <br>";                   // output : My gpa is 10.0
        echo "The GOD is {$god} <br>";                 // output : The GOD is 1, (true --> 1)
    ?>
    
<br>

### Arithmetic Operators
> +, -, *, /, **, %

        <?php

            $x = 5;
            $y = 5;
            $z = null;

            $z = $x + $y;
            echo $z; // output : 10

            $z = $x - $y;
            echo $z; // output : 0

            $z = $x * $y;
            echo $z; // output : 25

            $z = $x / $y;
            echo $z; // output : 1

            $z = $x ** $y;
            echo $z; // output : 3125

            $z = $x % $y;
            echo $z; // output : 0
        ?>
        
<br>

### Operator Precedence
> (), **, * / %, + - 

        <?php
            $maths_equation = 1 + 2 - (3 * 4) / 5 ** 6;
            echo $maths_equation; // output : 2.999232
        ?>
