# Component Lifecycle / `useEffect()` Hook

### Review, Research, and Discussion

1. Why do we not need more .html pages in a multi-page React app?

- becuase the React is a single page application and only contains and renders one HTML page always.

2. If we wanted a component to show up on every page, where would we put it and why? Outside the <BrowserRouter/>, Inside the <BrowserRouter />, outside a <Route /> ,Inside a <Route />

- will be inside the Route that will be as an instance of BrowserRouter, to allow the React App render needed component that is exisiting inside the Route, and each time the active route "by path" will be rendered.

3. What does routing do with the components that were rendered when a new route is requested
- in switch component from React-router, first route will match the clicked path will be rendered, and will go out the switch and will not see or render the other components.

4. What does props.children contain?
- we get props.childern by components composition and contains all props or things that the parent component has in JSX or render region.

5. How do useState() and this.setState() differ?

- setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

### Document the following Vocabulary Terms 

1. State Hook 
- built in function in react that allows you to add and update states to your stateless components. 

2. Mounting and Un-Mounting
- "mounting" (adding nodes to the DOM) or render the component, "unmounting" (removing them from the DOM) stop render or unrender the component , and "updating" (making changes to nodes already in the DOM) or edit the exist render of component. 