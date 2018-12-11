"# csci3055_finalproject" 

# Swift

## Introduction

  Swift is a programming language developed by Apple Inc for iOS, macOS, watchOS, tvOS, Linux and z/OS. Swift is also open-source with its source code divided into multiple open source repositories hosted on Github.

## Syntax

  Let's start with a simple print statement, in Swift to print is pretty simple 
  `print("hello world")`
  Like Python3 and Java, functions require braces `()` to accept parameters, in this case the string "hello world" was passed as a parameter into the print function. Swift uses similar syntax to its predecessor Objective-C. Unlike Java, it is optional to add semicolons after each statement in your code in Swift, but if you put use multiple statements in one line, a semicolon will be required to separate each statement `var HelloWorld = "Hello World!" ; print(HelloWorld)`. What is interesting about Swift is that unlike Python and Java, there must be an equal number of whitespace before and after an operator. For example, `print(1+2)` and `print(1 + 2)` are valid statements but `print(1 +2)` is not valid.
  
  When declaring variables, there are a couple ways to do it. One way is `var Variable: Double = 0.0` and another way is `var Variable = 0.0`. The reason why the second way is valid is because the Swift compiler has a feature called *type inference* where it can *infer* what type of variable it is based on the value you assign it. Another way of declaring a variable is `let Variable = 0.0`, but the variable declared will be immutable or constant and wouldn't be desired if it needs to be changed later on. An interesting fact is that with Swift, almost any character can be used for constant and variable names, including unicode characters.
```
let 🚽 = "toilet"
var 🔥💦 = "firewater"
print("\(🚽)")
print("\(🔥💦)")
```
 
When executed will print
```
toilet
firewater
```

This can be useful if there are developers that speak a non english language and their language can be typed out in unicode
`let 你好 = "你好世界"`
  
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

In Swift, there are a couple ways of using loops. Here's the syntax of a while loop:
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
Like the if statement, brackets are optional for while loops, but otherwise remain syntactically similar to Java.
The syntax of for-in loops in Swift is similar to for loops in Python. The only difference is that unlike Python, opening and closing brackets are required in for-in loops in Swift.
```
for index in variable {
  statement(s)
}
```

An example of a for-in loop in Swift:
```
var intList = [10,11,12,13,14]
for i in intList {
  print("Value of index is \(i)")
}
```
Resulting output:
```
Value of index is 10
Value of index is 11
Value of index is 12
Value of index is 13
Value of index is 14
```

Another example of for-in loop in Swift:
```
let range: CountableClosedRange = 1...5
for i in range {
  print("Value of i is \(i)")
}
```
Resulting output:
```
Value of i is 1
Value of i is 2
Value of i is 3
Value of i is 4
Value of i is 5
```
Swift does not support implicit type conversion so variables and constants have to be converted to the right type explicity `i = 1; Double(i)`. For string interpolation we would use `\()` to insert variable values into string literals.

Another interesting fact of Swift's syntax is its use of ranges. The most common forms of ranges are *Closed Ranges* and *Half Open Ranges*. Closed ranges use the `a...b` operator where it will create a Swift range that includes both element *a* and element *b*.  As shown in the example above, a range variable of type `CountableClosedRange` is declared that allows iteration. A variable of type `ClosedRange` allows access of elements within its range, but is not iterable because it is not part of the *Sequence Protocol* in Swift. Half-Open ranges use the `a..<b` operator which creates a range from element *a* up to but not including element*b*. Half-open ranges can be declared as `Range` or as `CountableRange`. Like closed ranges, `Range` is not iterable, but `CountableRange` is iterable.
