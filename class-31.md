# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-30) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-32)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Why do we not need more .html pages in a multi-page React app?

because we can use the react router in one page which will render whatever components are inside without the need to create a new html page.
2. If we wanted a component to show up on every page, where would we put it and why?
Outside the `<BrowserRouter/>`
Inside the `<BrowserRouter />`, outside a `<Route />`
Inside a `<Route />`  

Inside the `<BrowserRouter />`, outside a `<Route />`
because the react render method takes one child and i would put the child components in the `<BrowserRouter />` and outside the `<Route />` to be able to keep the components state  
3. What does props.children contain?
everything inside the component.  

## Terms

Composition: how components are build from other components, of varying complexity and specialization through props.  
Children / Child Components: first level descendant of a component  
Hash Routing: pouting that handles dynamic requests.  
Link Routing: routing that handles static requests.  

## hooks

Hooks let us organize the logic **inside** a component into reusable isolated units  

hooks are used when it is hard to apply the seperation of concerns principle because of the component complexity, such as in animations, form handling, connecting to external data sources.  

built-in React Hooks like `useState` and `useEffect` serve as the basic building blocks.  

```javascript
function Example() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

this example will be equalevent to the following:

```javascript
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```
