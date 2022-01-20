### Conceptual Exercise

Answer the following questions below:

- What is Redux? Why might you use it?
  Redux is used to handle state in react, traditionally state was passed from component to component from the top down
  Redux allows all components access to a centralized state store and therefore avoids propr drilling

- What are three features of the Redux developer tool in Chrome?
  tracing actions,skipping actions, preserving state

- What is a store?
  a centralized source of state data

- What is a reducer?
  a reducer is a pure function that takes an action and the previous state of the application and returns the new state 

- What is an action?
  Actions are a plain JavaScript object that contains information. Actions are the only source of information for the store. Actions have a type field that tells what kind of action to perform and all other fields contain information or data.

- What is an action creator?
  We frequently have action creators that we want to bind to the store. It may sound a bit complicated, but it is just creating a new "wrapper" function that does the store.dispatch() part. Since this is something we frequently need to do when using Redux, the library includes a function for this called: bindActionCreators().It's just a utility that takes an action creator (or a whole object of action creators) and binds them all to the dispatch function you got from a store.

- How does data flow in a React/Redux application?
  Redux follows the unidirectional data flow. It means that your application data will follow in one-way binding data flow. As the application grows & becomes complex, it is hard to reproduce issues and add new features if you have no control over the state of your application.

- What is the purpose of the `<Provider>` component?
  The <Provider> component makes the Redux store available to any nested components that need to access the Redux store.

- What is the purpose of the `useSelector` hook? What does it return?
  The equivalent of map state to props is useSelector. It takes in a function argument that returns the part of the state that you want. 

- Describe the `useDispatch` hook. What do you use it for?
  This hook returns a reference to the dispatch function from the Redux store. You may use it to dispatch actions as needed

- What is redux-thunk and why would you use it?
  Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed.

- What are propTypes?
  PropTypes is React's internal mechanism for adding type checking to components. React components use a special property named propTypes to set up type checking. When props are passed to a React component, they are checked against the type definitions configured in the propTypes property.

- Describe the `useCallback` hook.  What is it used for?
  The React useCallback Hook returns a memoized callback function. Think of memoization as caching a value so that it does not need to be recalculated. This allows us to isolate resource intensive functions so that they will not automatically run on every render The useCallback Hook only runs when one of its dependencies update. This can improve performance.

- Compare and contrast the `useReducer` hook with Redux (including react-redux).  Why would you choose one over the other?
  thorough discusion in this article https://www.robinwieruch.de/redux-vs-usereducer/