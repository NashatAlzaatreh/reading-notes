# Expressions and Operators and Loops

## ***Operators**
### JavaScript has the many types of operators. This section describes some of the operators and contains information about operator precedence.

- #### Assignment operators
- #### Comparison operators
- #### Arithmetic operators
- #### Logical operators

### Assignment operators:
#### An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal `(=)`, which assigns the value of its right operand to its left operand. That is, `x = y` assigns the value of `y` to `x`.

### Example of Compound assignment operators:

Name | Shorthand operator | Meaning
------------ | -------------   | ------------- 
Assignment| x = y	| 	x = y 
Addition assignment | x += y	| x = x + y
Multiplication assignment| x *= y | x = x * y  
Logical AND assignment| 	x &&= y	| x && (x = y)

#### Example of Compound assignment operators:
![Example of Compound assignment operators:](https://slidetodoc.com/presentation_image/f7a7a18267618b101da8576ee758d823/image-6.jpg)

## ***Expressions**
### An expression is any valid unit of code that resolves to a value.

#### Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value.

#### The expression `x = 7` is an example of the first type. This expression uses the `=` operator to assign the value seven to the variable `x`. The expression itself evaluates to seven.

#### The code `3 + 4` is an example of the second expression type. This expression uses the `+` operator to add three and four together without assigning the result, seven, to a variable.

### JavaScript has the following expression categories:

- #### Arithmetic: evaluates to a number, for example 3.14159. (Generally uses arithmetic operators.)
- ####  String: evaluates to a character string, for example, "Fred" or "234". (Generally uses string operators.)
- ####  Logical: evaluates to true or false. (Often involves logical operators.)
- ####  Primary expressions: Basic keywords and general expressions in JavaScript.
- ####  Left-hand-side expressions: Left values are the destination of an assignment.

## ***Loops**
		
#### Loops offer a quick and easy way to do something repeatedly.

#### You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop: 

```md
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
```
## for statement

A `for` loop repeats until a specified condition evaluates to `false`. The JavaScript `for` loop is similar to the Java and C `for` loop.

A `for` statement looks as follows:

```md
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
  ```
### When a for loop executes, the following occurs:

1. #### The initializing expression `initialExpression`, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
1. #### The `conditionExpression` expression is evaluated. If the value of `conditionExpression` is true, the loop statements execute. If the value of condition is false, the `for` loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
1. #### The `statement` executes. To execute multiple statements, use a block statement `({ ... })` to group those statements.
1. #### If present, the update expression `incrementExpression` is executed.
1. #### Control returns to Step 2.

## while statement

A `while` statement executes its statements as long as a specified condition evaluates to `true`. A `while` statement looks as follows:

```
while (condition)
  statement
```

#### If the `condition` becomes `false`, `statement` within the loop stops executing and control passes to the statement following the loop.

#### The condition test occurs before `statement` in the loop is executed. If the condition returns `true`, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following `while`.

#### To execute multiple statements, use a block statement `({ ... })` to group those statements.

