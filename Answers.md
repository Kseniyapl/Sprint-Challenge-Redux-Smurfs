1. Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?

  Map, filter, and reduce are 3 array methods. The map method creates a new object while extending the properties of another object.

2.  Describe actions, reducers and the store and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

    -Actions are set by the user during interaction with the website. Actions holds information about changes and description of that changes and can return JS objects and functions

    -Reducers are functions. Actions are dispatched through the reducers. Reducers always return a new object without influencing the intital state. 

    -Store is an object with methods that holds the state of the application. The only way to influence the state is to dispatch an action.

  In React-Redux applications, when your Redux is a single source of truth, it means that the only way to change your data in UI is to dispatch redux action which will change state within redux reducer. And your React components will watch this reducer and if that reducer changes, then UI will change itself too. But never other way around, because Redux state is single source of truth.

3. What is the difference between Application state and Component state? When would be a good time to use one over the other?

    -Application state is global state and (as parent) passes down state to all components(children).
    -Component State is local state that cannot be seen outside of the component.

4. What is middleware?

  Middleware provides a way to interact with actions that have been dispatched to the store before they reach the store's reducer.

5. Describe redux-thunk, what does it allow us to do? How does it change our action-creators? 

  Redux-thunk is a middleware that lets you call action creators that return a function instead of an "action" object.It can delay the dispatch of an action or dispatch the action in a moment when the specific condition is occurred.

6. Which react-redux method links up our components with our redux store?

  Connect() links up components with the redux store.
