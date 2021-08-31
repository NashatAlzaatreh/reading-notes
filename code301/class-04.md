# React and Forms

## React Docs - Forms

### 1- What is a ‘Controlled Component’?

#### keeping the form data in the component's state. In a controlled component, the form element's data is handled by the React component (not DOM) and kept in the component's state

### 2- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

#### We should update the state with their responses as soon as they enter them it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.

### 3- How do we target what the user is entering if we have an event handler on an input field?

#### handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

#### With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

## The Conditional (Ternary) Operator Explained

### 1- Why would we use a ternary operator?

#### To shorten your if statements into one line of code with the conditional operator

### 2- Rewrite the following statement using a ternary statement:

```javaScript
if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

### Answer :

```javaScript

ternary = x===y ? console.log(true) : console.log(false)

```
