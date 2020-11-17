# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-28) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-30)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Do child components have direct access to props/state from the parent?
yes
2. When a component “wraps” another component, how does the child component’s output get rendered?

```javascript
<Main>
  <Content />
</Main>
```

3. Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
yes
4. What trick can a parent use to share all props with it’s children?
Using React.Children to iterate over children and clone them with new props

## Terms

props.children: anything inside a parent component  
composition: give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way.

## Routing

For browser based projects, there are `<BrowserRouter>`(handle dynamic requests) and `<HashRouter>`(should be used for static websites ) components.  
Router components only expect to receive a single child element.  
