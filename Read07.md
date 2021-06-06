# Functions
#### Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

![function](https://raw.githubusercontent.com/learn-co-curriculum/cssi-2.3-functions/master/images/functions.png)

## Defining functions
### Function declarations
#### A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- #### The name of the function.
- #### A list of parameters to the function, enclosed in parentheses and separated by commas.
- #### The JavaScript statements that define the function, enclosed in curly brackets, `{...}`.

For example, the following code defines a simple function named `square`:
```
function square(number) {
  return number * number;
}
```  
#### The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:

```
return number * number;
```

### Function expressions

#### While the function declaration above is syntactically a statement, functions can also be created by a function expression.

#### Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:

```
const square = function(number) { return number * number }
var x = square(4) // x gets the value 16
```
#### However, a name can be provided with a function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

```
const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) }

console.log(factorial(3))
```

## Control flow
#### The control flow is the order in which the computer executes statements in a script.

#### Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

#### For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:

```
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
```
