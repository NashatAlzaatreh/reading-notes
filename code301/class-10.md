# In memory storage

## Understanding the JavaScript Call Stack

### - What is a ‘call’?

#### The call() allows for a function/method belonging to one object to be assigned and called for a different object. call() provides a new value of this to the function/method. With call() , you can write a method once and then inherit it in another object, without having to rewrite the method for the new object.

### - How many ‘calls’ can happen at once?

#### The maximal number of nested calls (including the first one) is called recursion depth. In our case, it will be exactly n . The maximal recursion depth is limited by JavaScript engine. We can rely on it being 10000, some engines allow more, but 100000 is probably out of limit for the majority of them

### - What does LIFO mean?

#### LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### - Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```JavaScript
function aFunction(){

console.log(“Hello from aFunction”); }

function bFunction(){

aFunction();

console.log(“The end from bFunction”); }

bFunction();
```

### - What causes a Stack Overflow?

#### A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## JavaScript error messages

### - What is a ‘refrence error’?

#### when you try to use a variable that is not yet declared you get this type os errors.

### - What is a ‘syntax error’?

#### are mistakes in using the language. Examples of syntax errors are missing a comma or a quotation mark, or misspelling a word.

### - What is a ‘range error’?

#### It's means when you invalid length to an object with some kind of length.

### - What is a ‘tyep error’?

#### this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible.

### - What is a breakpoint?

#### In software development, a breakpoint is an intentional stopping or pausing place in a program, put in place for debugging purposes. It is also sometimes simply referred to as a pause. More generally, a breakpoint is a means of acquiring knowledge about a program during its execution.

### - What does the word ‘debugger’ do in your code?

#### The easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again.
