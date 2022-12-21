# Learn Scala!
Hello! My name is Megan McNamara.
Together we will walk through the Scala programming langauge starting with how to download and create your first Hello World program. 

Scala can be installed on Windows, MacOS, and Linux. It can be run on VS Code (with the Metals extension), Atom, Sublime Text and more via the Langauge Server Protocol. 


## What is Scala?

Created in 2001, Scala was made to address the many criticisms of Java. It was made to show it's possible to combine functional and object-orientated programming. The name “Scala” is made from the words “scalable” and “language”, showing that it is designed to grow with the users. Scala is used for web development, data processing and distributed computing.


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
Just like Java, C and C++, Scala is staticly typed. This means the compiler determines the type of variable at compile time. If there are errors, it will fail to compile till the errors have been fixed. 

It is a case senstive language - if a variable is named "Hello" and you try using "hello" it would be two different variables.

### File Name
The Program File Name should exactly match the object name. Save the file as the exact object name and .scala (Remember Scala is case-sensitive). If the object name and file name do not match the program will not compile. 
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
``` def main(args: Array[String]) ````







