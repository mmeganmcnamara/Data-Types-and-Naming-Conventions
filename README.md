# Learn Scala!
Hello! My name is Megan McNamara.
Together we will walk through the Scala programming langauge starting with how to download and create your first Hello World program. 

Scala can be installed on Windows, MacOS, and Linux. It can be run on VS Code (with the Metals extension), Atom, Sublime Text and more via the Langauge Server Protocol. 


## What is Scala?

Created in 2001, Scala was made to address the many criticisms of Java. It was made to show it's possible to combine functional and object-orientated programming. The name “Scala” is made from the words “scalable” and “language”, showing that it is designed to grow with the users. Scala is used for web development, data processing and distributed computing. [^1]


The official Scala website: https://www.scala-lang.org/


## Getting Started:
Install on Mac:
1. open the Terminal 
2. Run 
```
brew install coursier/formulas/coursier && cs setup Coursier 
```
Java 8 or Java 11 and sbt are the tools needed to compile, run, test and package a Scala project.

To write comments in Scala, use // (ex: //This is a comment)

## Data Types and Naming
Just like Java, C and C++, Scala is **staticly typed**. This means the compiler determines the type of variable at compile time. If there are errors, it will fail to compile till the errors have been fixed. 

It is a case senstive language - if a variable is named "Hello" and you try using "hello" it would be two different variables.



### File Name
The Program File Name should exactly match the object name. Save the file as the exact object name and .scala (Remember Scala is case-sensitive). If the object name and file name do not match the program will not compile. Imagine the object name is HelloWorld. Therefore the file name will be: 
```
HelloWorld.scala
```

### Class
A class is the template/blueprint that describes the behaviors and states that are related to the class. 

Class names should be start with an Upper case letter; if there are several words in the class name, each first letter should be capitalized. 
```
class FirstScalaClass
```

### Methods
You can think of a method as a behavior. Inside a method, all actions are executed, data is manipulated and logics are written. There can be many methods in a class. The method body is enclosed between braces { }.
All method names shuld start with a lower case letter. If multiple words are used in the method name, then the inner word's first letter should be Upper Case.
```
def myMethodName()
```
Scala starts processing from the main method. 
``` 
def main(args: Array[String]) 
```
### Functions
The keyword "def" is used to declare a function in Scala. Function names should follow lower camel case, but can have special characters like +,~,&,-,++,\,/, etc. The return type of parameters must be specificed when defining the function. Return type of a function is optional; if you don't specificy the return type, the default is Unit (equivalent to void in Java).
```
def function_name ([parameter_list]) : [return_type] = {

// function body

}
```
If the equal sign and body is not used, then implicitly method is declared abstract. 
![image](https://user-images.githubusercontent.com/113136952/209726077-add0c5b7-c843-475e-b645-3180547874ef.png)
[^3]

Below is a simple program to show the data types, copied from Geeks for Geeks. [^5]
```
// Scala program to illustrate Datatypes
object Test
{
def main(args: Array[String]) 
{
    var a: Boolean = true
    var a1: Byte = 126
    var a2: Float = 2.45673f
    var a3: Int = 3
    var a4: Short = 45
    var a5: Double = 2.93846523
    var a6: Char = 'A'
    if (a == true) 
    {
    println("boolean:geeksforgeeks")
    }
    println("byte:" + a1)
    println("float:" + a2)
    println("integer:" + a3)
    println("short:" + a4)
    println("double:" + a5)
    println("char:" + a6)
}
}
``` 
Ouput: 
```
boolean:geeksforgeeks
byte:126
float:2.45673
integer:3
short:45
double:2.93846523
char:A
```

### Arrays
Arrays are a data structure with a fixed-size collection of elements of the same data type. Instead of declaring items as thing0, thing1, etc., an array allows you to make one variable and store all of the items inside said variable using thing[0], thing[1], etc. The index(number)  of the first element(thing) of an array is 0. The total number of elements is the index minus one, since you start counting at zero. 
To create an array you must:
1. declare a variable to reference the array
2. specify the type of array the variable can reference

The Syntax of an array: 
```
var z:Array[String] = new Array[String](3)

or

var z = new Array[String](3)
```
In this, z is declared as an array of Strings that has a maximum of 3 elements. You can 



## Variables
You can think of variables as storage locations. Every variable is known by its name and stores known and unknown information known as a value. A variable is defined by its data type and name. The data type is responsible for allocating memory for said variable. 
* Variable name can contain letter, digit, underscore ( _ ) and $
* White space is not allowed in the variable name
* Starting character of variable name must be a letter
* Variable name should be lower case

Scala has two types of variables:

1. Mutable Variable - variables whos value is able to be changed after the declaration of a variable. It is defined by the "var" keyword. The first letter of a data type needs to be a capital letter, since Scala treats data types as objects. 
```
var name: String = "value";
```

2. Immutable Variables - variables whos value is NOT changable after declaration of a variable. It is defined by the "val" keyword. The first letter of a data type needs to be a capital letter, since Scala treats data types as objects. "Val" is similar to "final" in Java. [^2]
```
val name: String = "value";
```

### Conditional Statements
Scala has 4 conditional statements. 
- If
- If-else
- Nested If-else
- If-else Ladder 


"If" statement consists of a Boolean expression followed by one or more statements. If the Boolean expressions evaluates to true then the code inside the "if" will be executed. If not, the set of code after the closing curly brace will be executed. 
![image](https://user-images.githubusercontent.com/113136952/209727349-4d5f157f-bf23-4aa4-b7fe-60193e93cee0.png) [^4]

Here is an example of a simple if statement:
```
var x = 10;

      if( x < 20 ){
         println("This is an if statement");
      }
```
It will output "This is an if statement" because the statement was true. 

If-else is very similar to an if statement, however if the boolean statement is false, it will execute the else statement. Think of it as "if this is true do this, else do this".
```
var x = 30;

      if( x < 20 ){
         println("This is an if statement");
      } else {
         println("This is an else statement");
      }
 ```
Output: 
```
This is an else statement
```

Nested if-else statements are for when you want an if-else statement inside of another if-else statement. [^7]
```
 // taking three variables
    var a: Int = 70
    var b: Int = 40
    var c: Int = 100
  
    // condition_1
    if (a > b) 
    {
        // condition_2
        if(a > c)
        {
            println("a is largest");
        }
        else
        {
            println("c is largest")
        }
      
    }
      
    else
    {
          
         // condition_3
        if(b > c)
        {
            println("b is largest")
        }
        else
        {
            println("c is largest")
        }
    }
``` 
Output: 
``` 
c is largest
```

If-else ladder is used when the user wants to deciede from multiple options. The if statements are executed from the top down. As soon as one of the conditions controlling the if is true, the statement associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final else statement will be executed. [^7]
```
// Taking a variable
    var value: Int = 50
  
    if (value == 20) 
    {
  
        // print "value is 20" when 
        // above condition is true
        println("Value is 20")
    } 
      
    else if (value == 25) 
    {
  
        // print "value is 25" when 
        // above condition is true
        println("Value is 25")
    } 
      
    else if (value == 40)
    {
      
        // print "value is 40" when 
        // above condition is true
        println("Value is 40")
  
    } 
      
    else 
    {
          
        // print "No Match Found" 
        // when all condition is false
        println("No Match Found")
    }
```
Output:
```
No Match Found
```
### Short Circuit
Short circuiting is when the program stops further evaluation of booleans as soon as the result is known. [^8]
Logical operators, such as && and ||, are short-circuit operators.



[^1]: https://docs.scala-lang.org/getting-started/index.html
[^2]: https://www.geeksforgeeks.org/variables-in-scala/
[^3]: https://medium.com/analytics-vidhya/scala-basics-ace1dccd72f8#:~:text=Case%20Sensitivity%20%E2%88%92%20Scala%20is%20case,have%20different%20meaning%20in%20Scala.
[^4]: https://www.tutorialspoint.com/scala/scala_if_else.htm
[^5]: https://www.geeksforgeeks.org/data-types-in-scala/?ref=lbp
[^6]: https://www.tutorialspoint.com/scala/scala_arrays.htm
[^7]: https://www.geeksforgeeks.org/scala-decision-making-if-if-else-nested-if-else-if-else-if/
[^8]: https://rosettacode.org/wiki/Short-circuit_evaluation#Scala




