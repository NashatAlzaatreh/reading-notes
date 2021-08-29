# State and Props
## State and Lifecycle




### Using State Correctly

- There are three things you should know about `setState()`.

    1. Do Not Modify State Directly  
        this is wrong: `this.state.comment = 'Hello';`  
        instead : `this.setState({comment: 'Hello'});`  
        - The only place where you can assign this.state is the constructor.

    1. State Updates May Be Asynchronous  
        React may batch multiple `setState()` calls into a single update for performance.   
        Because `this.props` and `this.state` may be updated asynchronously, you should not rely on their values for calculating the next state.  
        - this fails: `this.setState({counter: this.state.counter + this.props.increment,});`  
        - this works: `this.setState((state, props) => ({  counter: state.counter + props.increment`
    1. State Updates are Merged  
        - When you call `setState()`, React merges the object you provide into the current state.


### State vs Props 

#### Props 
##### Short for properties, props can best be defined as a way of passing data from component to component, basically from parent to child component. 

#### State 
##### If props hold immutable data and are rendered by components, then state stores data about the component that can change over time. Change could come in the form of user events or system events such as response to user input or server requests. Working with a state’s component normally involves setting a component’s default state, accessing the current state and updating the state. I think the most suitable way to explain state in React would be the demo of a counter.
  
  ![State vs Props ](https://i.stack.imgur.com/G8Kj0.png)

   ![State vs Props ](https://coding.degree/wp-content/uploads/2020/10/img_5f8ea9fe3260c.png)


  

### render():
##### Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false.

### componentDidMount() :
##### This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
##### setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.
        
### Adding Lifecycle Methods to a Class

- Whenever a component is changed, after it's rendered to the DOM for the first time. It is called “mounting” in React.

- We call clearing changes, whenever the DOM produced by the component is removed. “unmounting” in React.

- A pair of “**mounting**” and “**unmounting**” is called the **lifecycle methods**


### The Data Flows Down

- Neither parent nor child components can know if a certain component is stateful or stateless, and they shouldn’t care whether it is defined as a function or a class.

- In React apps, whether a component is stateful or stateless is considered an implementation detail of the component that may change over time. You can use stateless components inside stateful components, and vice versa.

## Handling Events

- There are some syntax differences between **React** events and the **DOM** events:
    1. React events are named using camelCase, rather than lowercase.
    1. With JSX you pass a function as the event handler, rather than a string.

- In the **DOM** way:   


```
<button onclick="activateLasers()">
  Activate Lasers
</button>

```

- In the **React** way:  

```
<button onClick={activateLasers}>
  Activate Lasers
</button>

```

- Another difference is that you cannot return false to prevent default behavior in React. You must call `preventDefault` explicitly.

- When using React, you generally don’t need to call `addEventListener` to add listeners to a DOM element after it is created. Instead, just provide a listener when the element is initially rendered.


### Conditional Rendering

- In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

- Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like `if` or the `conditional operator` to create elements representing the current state, and let React update the UI to match them.


  
  
### Preventing Component from Rendering

- In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return `null` instead of its render output.

- Returning `null` from a component’s render method does not affect the firing of the component’s lifecycle methods. For instance function that responsible for rendering the component will still be called.
