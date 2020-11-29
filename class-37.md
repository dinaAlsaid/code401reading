# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-34) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-36)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Why choose Redux instead of the Context API for global state?  
because of readability and performance issues. and context API Does Not Separate Logic From Presentation
2. What is the purpose of a reducer?  
take the current state and an action as arguments, and return a new state result.  
3. What does an action contain?  
a type and payload.  
4. Why do we need to copy the state in a reducer?  

## Term

- immutable state:read only.
- time travel in redux: going back to a previous state
- action creator:  
- reducer: a pure function that takes the previous state the dispatched action and returns the next state.
- dispatch: fire an action to change a state

## combineReducers

helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

Any reducer passed to combineReducers must satisfy these rules:

- For any action that is not recognized, it must return the state given to it as the first argument.
- It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.
- If the state given to it is undefined, it must return the initial state for this specific reducer. According to the previous rule, the initial state must not be undefined either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being undefined.  
