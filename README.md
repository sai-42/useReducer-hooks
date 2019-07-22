`useReducer`

```js
const [state, dispatch] = useReducer(reducer, initialArg, init);
```

An alternative to `useState`.
Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.

`useReducer` is usually preferable to `useState` when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
`useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.
