"# csci3055_finalproject" 

# Swift

## Introduction

  Swift is a programming language developed by Apple Inc for iOS, macOS, watchOS, tvOS, Linux and z/OS. Swift is also open-source with its source code divided into multiple open source repositories hosted on Github.

## Syntax

  Let's start with a simple print statement, in Swift to print is pretty simple 
  `print("hello world")`
  Like Python3 and Java, functions require braces `()` to accept parameters, in this case the string "hello world" was passed as a parameter into the print function. Swift uses similar syntax to its predecessor Objective-C. Unlike Java, it is optional to add semicolons after each statement in your code in Swift, but if you put use multiple statements in one line, a semicolon will be required to separate each statement `var HelloWorld = "Hello World!" ; print(HelloWorld)`. What is interesting about Swift is that unlike Python and Java, there must be an equal number of whitespace before and after an operator. For example, `print(1+2)` and `print(1 + 2)` are valid statements but `print(1 +2)` is not valid.
  
Here's the syntax of an if-statement:
```
if (expression) {
  statement(s)
}
```
Here's the syntax of an if-else statement:
```
if (expression) {
  statement(s)
}
else {
  statement(s)
}
```
where the statements in else are executed if the expression is not true. Here's the syntax of an if-else-if statement:
```
if (expression) {
  statement(s)
}
else if (expression2) {
  statement(s)
}
else {
  statement(s)
}
```
An example of an if-else statement is
```
var i = 10
if i == 10 {
  print("This number is 10")
}
else {
  print("This number is not 10")
}
```
Which will print out
```
This number is 10
```
Brackets are optional in if statements. If statements in Swift are very similar to Java with one difference being that brackets are required around expressions in if statements in java while in Swift it is optional.
Here's the syntax of a while loop:
```
while condition {
  statement(s)
}
```
And an example of a while loop
```
var i = 0

while i < 10 {
  print ("i is \(i)")
  i = i + 1
}
```
Which will print out:
```
i is 0
i is 1
i is 2
i is 3
i is 4
i is 5
i is 6
i is 7
i is 8
i is 9
```
