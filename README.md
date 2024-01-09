# react-snippets

---

<details>
<summary>Methods as props</summary>

  https://codesandbox.io/p/sandbox/method-as-prop-d4nn8m

</details>

----

<details>
<summary>Applying CSS</summary>
  
  https://codesandbox.io/p/sandbox/css-rl9p4t

</details>

---

<details>
<summary> Form handling </summary>
  
  https://codesandbox.io/p/sandbox/form-handling-gxvkn2
  
</details>

---

<details>
<summary>Pure component </summary>
  
https://codesandbox.io/p/sandbox/pure-components-dd4ck2
- Shallow comparisons, if no diff - then it will not re-render, including child which leads to the performance boost
- We should not mutate array/object, always return that reflects a new state (spread operator)
  
</details>

---

<details>
<summary>Memo </summary>
  
  https://codesandbox.io/p/sandbox/memo-n7xdr3
  - same as a pure component, but for the functional component
    
</details>


---

<details>
<summary>Ref </summary>

https://codesandbox.io/p/sandbox/refs-w63tpl
  - attached to a React element and used to interact with the underlying DOM
  - Example: Focus

  
</details>

---


<details>
<summary> Portals </summary>
  
https://codesandbox.io/p/sandbox/portals-t2y3x6
  - way to render children components at a different place in the DOM (Document Object Model) hierarchy than the parent component (root)
  - we can apply different CSS (root vs portal-root)

</details>

---

<details>
<summary> Error boundary </summary>

https://codesandbox.io/p/sandbox/error-boundary-jkfcg8
  - use for fallback UI or log the error.
  - the class component that implements either one or both lifecycle methods `getDerivedStateFromError` or `componentDidCatch` becomes an error boundary.
  - do not catch errors in the event handler, use try catch in case of an event handler.

</details>


---

<details>
<summary>Higher order component (hoc) </summary>

https://codesandbox.io/p/sandbox/higher-order-component-hoc-2774zg
  - used to share common functionality between components
  - pattern where function takes a component as an argument and returns a new component

</details>

---

<details>
<summary>Context </summary>

https://codesandbox.io/p/sandbox/context-7dxg6v
  - provides a way to pass data through the component tree without passing props at every level
  - example: username, theme preference. 

</details>

---

<details>
<summary>HTTP Request </summary>
  
https://codesandbox.io/p/sandbox/request-qg54cs
  - axios for request
  - redux axios middleware when using with redux
  - formik for building form (validation)

</details>

---


<details>
<summary>useEffect </summary>
 
 https://codesandbox.io/p/sandbox/useeffect-ww8q4p
  - similar to `componentDidMount` and `componentWillUnmount`
  - second argument will be dependencies

</details>

---

<details>
<summary>useContext </summary>
  
https://codesandbox.io/p/sandbox/usecontext-7r7d9x

</details>


---

<details>
<summary>useReducer </summary>
  
https://codesandbox.io/p/sandbox/usereducer-58k9s3
  - [reducer](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)
  - | **Case**                  | **useState**      | **useReducer**         |
    |---------------------------|-------------------|------------------------|
    | type                      | num, bool, string | object, array          |
    | num of state transitions  | 1 or 2            | too many               |
    | business logic            | no business logic | complex business logic |
    | related state transitions | no                | yes                    |
    | use                       | local             | global                 |

</details>


---

<details>
<summary>useCallback </summary>
  
https://codesandbox.io/p/sandbox/usecallback-rgj34d
  -  used for optimization

</details>

---
<details>
<summary>useMemo </summary>
  
https://codesandbox.io/p/sandbox/usememo-w44w54
  - Used for performance optimization
  - if want to cache a function - use callback, if want to cache a result of a function - use memo

</details>

---
<details>
<summary>useRef </summary>
 
https://codesandbox.io/p/sandbox/useref-hpgc8h
  - same as refs

</details>

---

<details>
<summary>Controlled and Uncontrolled Components </summary>
  
- Controlled : state is managed by react
```jsx
const handleChange = (event) => {
  setValue(event.target.value);
};
```
- Uncontrolled : state is managed by dom
```jsx
  const handleClick = () => {
  alert(`Input value: ${inputRef.current.value}`);
  };
```

</details>

---

<details>
<summary>children prop </summary>
  
- special prop that allows components to include content or elements between their opening and closing tags
```jsx
const CompA = (props) => {
  return (
    <>
      <h2>{props.children} </h2> // will print 'hello bye'
    </>
  );
};
.
.
<CompA> hello bye </CompA>
```

</details>

--- 

<details>
<summary> React.Fragment </summary>
  
- return multiple elements without using `<div></div>`
  ```jsx
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
    </React.Fragment>
  )
  ```
  or
  ```jsx
  return (
    <>
      <ChildA />
      <ChildB />
    </>
  )
  ```
  
</details>
--- 

<details>
<summary> TODO </summary>
  - React.lazy with example (suspense)

  <details>
    <summary>  </summary>
      
    </details>

</details>




