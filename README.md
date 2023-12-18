# react-snippets

---

#### Methods as props
https://codesandbox.io/p/sandbox/method-as-prop-d4nn8m


---
#### Applying CSS
https://codesandbox.io/p/sandbox/css-rl9p4t

---
#### Form handling
https://codesandbox.io/p/sandbox/form-handling-gxvkn2

---
#### Pure component
https://codesandbox.io/p/sandbox/pure-components-dd4ck2
  - Shallow comparisons, if no diff - then it will not re-render, including child which leads to the performance boost
  - We should not mutate array/object, always return that reflects a new state (spread operator)

---
#### Memo
https://codesandbox.io/p/sandbox/memo-n7xdr3
  - same as a pure component, but for the functional component

---
#### Refs

https://codesandbox.io/p/sandbox/refs-w63tpl
  - attached to a React element and used to interact with the underlying DOM
  - Example: Focus

---
#### Portals
https://codesandbox.io/p/sandbox/portals-t2y3x6
  - way to render children components at a different place in the DOM (Document Object Model) hierarchy than the parent component (root)
  - we can apply different CSS (root vs portal-root)

---
#### Error boundary
https://codesandbox.io/p/sandbox/error-boundary-jkfcg8
  - use for fallback UI or log the error.
  - the class component that implements either one or both lifecycle methods `getDerivedStateFromError` or `componentDidCatch` becomes an error boundary.
  - do not catch errors in the event handler, use try catch in case of an event handler.

---
#### Context
https://codesandbox.io/p/sandbox/context-7dxg6v
  - provides a way to pass data through the component tree without passing props at every level
  - example: username, theme preference. 
---
####  HTTP Request 
https://codesandbox.io/p/sandbox/request-qg54cs
  - axios for request
  - redux axios middleware when using with redux
  - formik for building form (validation)
