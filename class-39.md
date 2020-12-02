# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-37) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-41)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?  
   use life cycle hooks of a higher order component and using thunk as a middleware
2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
   the thunk/async function

## terms

middleware: the layer between the application layer and the server
thunk: an asynchronous function that enables a redux app to dispatch an action asynchronously

## RTK

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address common concerns about Redux like:

- Configuring a Redux store is too complicated
- I have to add a lot of packages to get Redux to do anything useful

Other State managers:

- Mobx
- HookState
