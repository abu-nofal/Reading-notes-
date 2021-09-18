# Context API

---
### Review, Research, and Discussion

--- 
**Describe use cases useState() vs useReducer()**

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

**Why do custom hooks need the use prefix?**

- Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

**What do custom hooks usually do?**

- Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

**Describe how a hook that fetches API data might work**

- aha you can use the useEffect than the method fetch with the url (its simller to axios and geting the data or request it )

[ref](https://designcode.io/react-hooks-handbook-fetch-data-from-an-api/)

--- 

### Document the following Vocabulary Terms

--- 
**reducer** 

- ***useReducer*** is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one 

