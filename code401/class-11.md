# Event Driven Applications

## Review, Research, and Discussion

#### Importance of access control

Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorization, unlawfully and the risk of a data breach.

#### Application that would need access control

Ant organization that consist of important data need to apply access control, Banks, Universities, social media platforms, online shops and etc.

#### Roles in Access Control

Normally used in `RBAC` or **Role-Based Access Control**, it's assigned to users to give each one special access permissions like read, write, update and delete.

#### Role-Based Access Control Scalability

## They reduce the tasks of an administrator or authorities when users take on different roles in an organization and need to be assigned different access rights or privileges based on these roles. RBAC is a very expressive and flexible access control mechanism that makes it possible to have security policies based on the principle of least privilege, static and dynamic separation of duties, conflicts between roles and permissions, and many more

## Terms

| term                      | definition                                                                                                                                                                         |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Authorization             | a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features. |
| Role Based Access Control | a security paradigm whereby users are granted access to resources based on their role in the company.                                                                              |
| Capabilities              | it's what the role in an RBAC system can do.                                                                                                                                       |

---

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?  
   SQL and Role Based Access Control.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   Event Driven Programming
1. What are you most excited about trying to implement or see how it works?
   Events.

---

### Event Driven Programming

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

Event-Driven Programming makes use of the following concepts:

An Event Handler is a callback function that will be called when an event is triggered.
A Main Loop listens for event triggers and calls the associated event handler for that event.

We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

```
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

Now we can get started with Event-Driven Programming in Node.

Imagine we’re creating a chat room. We want to alert everyone when a new user joins the chat room. We’ll need an event listener for a userJoined event. First, we’ll write a function that will act as our event listener, then we can use EventEmitters on method to set the listener.

```
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;

function userJoined(username){
// Assuming we already have a function to alert all users.
alertAllUsers('User ' + username + ' has joined the chat.');
}

// Run the userJoined function when a 'userJoined' event is triggered.
chatRoomEvents.on('userJoined', userJoined);
```

The next step would be to make sure that our chat room triggers a userJoined event whenever someone logs in so that our event handler is called. EventEmitter has an emit method that we we use to trigger the event. We would want to trigger this event from within a login function inside of our chatroom module.

```
function login(username){
chatRoomEvents.emit('userJoined', username);
}
```

We could expand further by creating events for when a user logs out, when a message is sent, when a message is received, or any other event we could possibly need for our chat room to be as dynamic as we want it.
