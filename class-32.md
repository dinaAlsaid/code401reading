# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-31) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-33)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. What does a component’s lifecycle refer to?  
   the component's mounting, updating and unmounting.
2. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect  
   it ensures the function is reacreated only when the state is updated.
3. Why are functional components preferred over class components?
   ability to use hooks therefore the ability to use the seperation of concerns principle
4. What is wrong with the following code?

```javascript
import React, { useState, useEffect } from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = [];

  for (let i = 0; i < count; i++) {
    useEffect(() => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (
    <div>
      <input type="number" value={count} onChange={changeCount} />
      {renderedItems}
    </div>
  );
}
```

## Terms

state hook: used for declaring and updating a state variable.
effect hook: a function used to add live cycle events for functional components.

## custom hooks and useReducer

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.  

```const [state, dispatch] = useReducer(reducer, initialArg, init);```  
useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.  

We cannot use 'async' keyword with 'useEffect' callback method.instead make a custom async hook.  

