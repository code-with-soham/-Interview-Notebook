# ═══════════════════════════════════════════════════════

# SECTION 3: REACT (COMPLETE)

# ═══════════════════════════════════════════════════════

---

## 3.1 React Fundamentals

### ✅ Important Topics

- [ ] What is React and why use it
- [ ] SPA (Single Page Application) vs MPA
- [ ] Declarative vs Imperative programming
- [ ] JSX (JavaScript XML)
- [ ] JSX compilation (Babel)
- [ ] React.createElement()
- [ ] React DOM
- [ ] React Fragments
- [ ] Strict Mode
- [ ] React 18 features (Concurrent Mode, Automatic Batching, Transitions)
- [ ] React 19 features (use hook, Server Components, Actions)

### 📋 Interview Questions

1. What is React? Why is it used?
2. What is a Single Page Application (SPA)?
3. What is the difference between a library and a framework? Is React a library or framework?
4. What is JSX? Is it mandatory to use JSX in React?
5. How does JSX get converted to JavaScript?
6. What is `React.createElement()`? What does it return?
7. What are React Fragments? Why are they used?
8. What is `<React.StrictMode>`? What does it do?
9. What is the difference between React and ReactDOM?
10. What is the significance of the `key` prop in React?
11. Why should you not use array index as `key`?
12. What is the difference between React and Angular?
13. What is the difference between React and Vue?
14. What are the advantages and disadvantages of React?
15. What is Concurrent Mode in React 18?
16. What is Automatic Batching in React 18?
17. What are Server Components in React?

### 🎯 Scenario Based Questions

18. When would you choose React over vanilla JavaScript for a project?
19. You have a list that updates frequently. How would you optimize rendering?
20. Your JSX is not rendering. What could be the common issues?

---

## 3.2 Components

### ✅ Important Topics

- [ ] Functional Components
- [ ] Class Components
- [ ] Component composition
- [ ] Higher-Order Components (HOC)
- [ ] Render Props
- [ ] Compound Components
- [ ] Controlled vs Uncontrolled Components
- [ ] Pure Components
- [ ] Component naming conventions
- [ ] Default props
- [ ] Children prop
- [ ] Component lifecycle (class-based)

### 📋 Interview Questions

1. What is a component in React?
2. What is the difference between functional and class components?
3. What are Higher-Order Components (HOC)? Give an example.
4. What is the Render Props pattern?
5. What is component composition? Why is it preferred over inheritance?
6. What are Compound Components?
7. What is the difference between controlled and uncontrolled components?
8. What is a Pure Component?
9. What is the `children` prop?
10. Can a component return multiple elements? How?
11. What happens if you don't return anything from a component?
12. What is the difference between a component and an element in React?
13. When should you split a component into smaller components?
14. What are default props? How do you set them?
15. What are the rules for creating a React component?

### 🔥 Frequently Asked Questions

16. Why are class components being replaced by functional components?
17. What is the difference between HOC and Render Props? When would you use each?
18. How do you share logic between components without HOC or Render Props?
19. Can you use hooks inside class components?
20. What is the difference between `React.Component` and `React.PureComponent`?

### 💻 Coding Questions

21. Create a Higher-Order Component that adds loading state to any component.
22. Implement a Render Props pattern for mouse tracking.
23. Create a compound component pattern for a Tabs component.
24. Convert a class component to a functional component with hooks.
25. Build a reusable Modal component.

---

## 3.3 Hooks (Complete)

### ✅ Important Topics

- [ ] useState
- [ ] useEffect
- [ ] useContext
- [ ] useReducer
- [ ] useRef
- [ ] useMemo
- [ ] useCallback
- [ ] useLayoutEffect
- [ ] useId
- [ ] useTransition
- [ ] useDeferredValue
- [ ] useImperativeHandle
- [ ] useDebugValue
- [ ] useSyncExternalStore
- [ ] useInsertionEffect
- [ ] Custom hooks
- [ ] Rules of Hooks

### 📋 Interview Questions — useState

1. What is `useState`? How does it work?
2. What is the initial state? Can it be a function?
3. Why does `useState` return an array and not an object?
4. What happens when you call the setter function with the same value?
5. What is the difference between `setState(newValue)` and `setState(prev => newValue)`?
6. Can you call `useState` conditionally? Why or why not?
7. How does React batch state updates?
8. What happens if you call `setState` multiple times in the same function?
9. Is `useState` synchronous or asynchronous?
10. How do you update an object or array in state correctly?

### 📋 Interview Questions — useEffect

11. What is `useEffect`? What does it replace from class components?
12. What is the dependency array in `useEffect`?
13. What happens if you pass an empty dependency array `[]`?
14. What happens if you don't pass a dependency array at all?
15. What is a cleanup function in `useEffect`? When does it run?
16. Can you use `async/await` directly inside `useEffect`?
17. What is the difference between `useEffect` and `useLayoutEffect`?
18. How do you avoid infinite loops in `useEffect`?
19. What are the common mistakes with `useEffect`?
20. How does React decide when to re-run an effect?
21. Can you have multiple `useEffect` hooks in one component?

### 📋 Interview Questions — useRef

22. What is `useRef`? How is it different from `useState`?
23. Does updating a ref trigger a re-render?
24. What are the use cases for `useRef`?
25. How do you access DOM elements using `useRef`?
26. What is the difference between `useRef` and `createRef`?
27. Can you use `useRef` to store the previous value of a state?
28. What is `forwardRef`? When is it needed?

### 📋 Interview Questions — useReducer

29. What is `useReducer`? When should you use it over `useState`?
30. What is the structure of a reducer function?
31. What is the `dispatch` function?
32. What is the difference between `useState` and `useReducer`?
33. Can you use `useReducer` with `useContext` to replace Redux?
34. What is lazy initialization in `useReducer`?

### 📋 Interview Questions — useContext

35. What is `useContext`? How does it work?
36. What problem does `useContext` solve?
37. What is prop drilling? How does Context API solve it?
38. What are the performance implications of using Context?
39. Does changing context value re-render all consumers?
40. How do you optimize Context to prevent unnecessary re-renders?

### 📋 Interview Questions — useMemo & useCallback

41. What is `useMemo`? When should you use it?
42. What is `useCallback`? When should you use it?
43. What is the difference between `useMemo` and `useCallback`?
44. When should you NOT use `useMemo` or `useCallback`?
45. What is referential equality and why does it matter in React?
46. How do `useMemo` and `useCallback` help with performance?
47. What happens if the dependency array is incorrect?

### 📋 Interview Questions — Custom Hooks

48. What are custom hooks?
49. What is the naming convention for custom hooks?
50. Why must custom hooks start with `use`?
51. Can custom hooks return JSX?
52. How do you share stateful logic using custom hooks?
53. Can you use hooks inside custom hooks?
54. What are some common custom hooks you've used or built?

### 📋 Interview Questions — Rules of Hooks

55. What are the Rules of Hooks?
56. Why can't you call hooks inside loops, conditions, or nested functions?
57. What ensures hooks are called in the right order?
58. What happens if you violate the Rules of Hooks?

### 🖥️ Output/Behavior Based Questions

59. What happens when you do this?

```jsx
const [count, setCount] = useState(0);
setCount(count + 1);
setCount(count + 1);
setCount(count + 1);
// What is the final value of count?
```

60. What happens when you do this instead?

```jsx
const [count, setCount] = useState(0);
setCount((prev) => prev + 1);
setCount((prev) => prev + 1);
setCount((prev) => prev + 1);
// What is the final value of count?
```

61. What is wrong with this code?

```jsx
useEffect(async () => {
  const data = await fetchData();
  setData(data);
}, []);
```

62. What happens here?

```jsx
const [count, setCount] = useState(0);
useEffect(() => {
  setCount(count + 1);
}, [count]);
```

63. What is the behavior?

```jsx
const ref = useRef(0);
ref.current = ref.current + 1;
console.log(ref.current);
// Does the component re-render?
```

64. What is wrong with this code?

```jsx
if (isLoggedIn) {
  const [user, setUser] = useState(null);
}
```

### 💻 Coding Questions

65. Build a custom `useLocalStorage` hook.
66. Build a custom `useFetch` hook with loading and error states.
67. Build a custom `useDebounce` hook.
68. Build a custom `useToggle` hook.
69. Build a custom `usePrevious` hook.
70. Build a custom `useOnClickOutside` hook.
71. Build a custom `useMediaQuery` hook.
72. Build a custom `useIntersectionObserver` hook.
73. Build a custom `useWindowSize` hook.
74. Build a custom `useInterval` hook.

---

## 3.4 Component Lifecycle

### ✅ Important Topics

- [ ] Mounting (constructor, render, componentDidMount)
- [ ] Updating (shouldComponentUpdate, render, componentDidUpdate)
- [ ] Unmounting (componentWillUnmount)
- [ ] Error handling (componentDidCatch, getDerivedStateFromError)
- [ ] Hook equivalents of lifecycle methods
- [ ] Lifecycle order

### 📋 Interview Questions

1. What are the lifecycle phases of a React component?
2. What lifecycle methods are called during mounting?
3. What lifecycle methods are called during updating?
4. What is `componentDidMount`? What is its hook equivalent?
5. What is `componentDidUpdate`? What is its hook equivalent?
6. What is `componentWillUnmount`? What is its hook equivalent?
7. What is `shouldComponentUpdate`? What is its hook equivalent?
8. What is `getDerivedStateFromProps`?
9. What is `getSnapshotBeforeUpdate`?
10. What is the order of lifecycle methods in a parent-child component tree?
11. How do you handle errors in React components?
12. What is `componentDidCatch`? What is `getDerivedStateFromError`?

---

## 3.5 Rendering & Reconciliation

### ✅ Important Topics

- [ ] React rendering process
- [ ] Trigger → Render → Commit phases
- [ ] Virtual DOM diffing
- [ ] Reconciliation algorithm
- [ ] Key prop and reconciliation
- [ ] Batching
- [ ] Re-renders (what causes them)
- [ ] Preventing unnecessary re-renders
- [ ] Strict Mode double rendering
- [ ] Concurrent rendering

### 📋 Interview Questions

1. How does React rendering work?
2. What is reconciliation?
3. What is the diffing algorithm in React?
4. What are the assumptions React's diffing algorithm makes?
5. How does the `key` prop affect reconciliation?
6. What causes a component to re-render?
7. Does a parent re-render cause all children to re-render?
8. How do you prevent unnecessary re-renders?
9. What is batching in React?
10. What is automatic batching in React 18?
11. What is the difference between the render phase and the commit phase?
12. Why does React's Strict Mode render components twice?
13. What is concurrent rendering?
14. What is the difference between `state` change and `props` change re-renders?

### 🎯 Scenario Based Questions

15. You have a component that re-renders 100 times per second. How do you optimize it?
16. A child component re-renders even though its props haven't changed. Why?
17. You moved state to a parent component and now the whole app re-renders. How do you fix it?
18. How would you use React DevTools to identify unnecessary re-renders?

---

## 3.6 React Fiber

### ✅ Important Topics

- [ ] What is React Fiber
- [ ] Fiber architecture
- [ ] Incremental rendering
- [ ] Work-in-progress tree
- [ ] Priority-based rendering
- [ ] Time slicing
- [ ] Interruptible rendering

### 📋 Interview Questions

1. What is React Fiber?
2. Why was Fiber introduced?
3. How does Fiber improve rendering performance?
4. What is incremental rendering?
5. What is the work-in-progress tree?
6. How does Fiber handle priority-based rendering?
7. What is time slicing in React?
8. What is the difference between the old (Stack) reconciler and Fiber?
9. How does Fiber enable concurrent features in React 18?

---

## 3.7 Virtual DOM

### ✅ Important Topics

- [ ] Virtual DOM representation
- [ ] How Virtual DOM works in React
- [ ] Diffing process
- [ ] Batch updates
- [ ] Virtual DOM vs Real DOM performance

### 📋 Interview Questions

1. What is the Virtual DOM in React?
2. How does the Virtual DOM improve performance?
3. How does React update the real DOM?
4. What is the diffing algorithm?
5. Is the Virtual DOM always faster than direct DOM manipulation?
6. What is a React Element? What does it look like internally?
7. How is the Virtual DOM different from the Shadow DOM?
8. Does React re-render the entire Virtual DOM on every state change?

---

## 3.8 State Management

### ✅ Important Topics

- [ ] Local state (useState)
- [ ] Component state vs Application state
- [ ] Lifting state up
- [ ] Context API
- [ ] Redux (Store, Actions, Reducers, Dispatch, Selectors)
- [ ] Redux Toolkit (RTK)
- [ ] Redux middleware (Thunk, Saga)
- [ ] Zustand
- [ ] React Query / TanStack Query
- [ ] Jotai, Recoil, MobX (awareness)
- [ ] When to use which state management

### 📋 Interview Questions — State Basics

1. What is state in React?
2. What is the difference between state and props?
3. Can you modify props directly? Why not?
4. What is "lifting state up"? When do you do it?
5. What is the difference between local state and global state?
6. When should you use local state vs global state?
7. What is prop drilling? How do you solve it?

### 📋 Interview Questions — Context API

8. What is the Context API?
9. How do you create and use a Context?
10. What is the Provider-Consumer pattern?
11. What are the limitations of Context API?
12. Why is Context API not a replacement for Redux?
13. How do you prevent unnecessary re-renders when using Context?
14. Can you have multiple Contexts in one application?

### 📋 Interview Questions — Redux

15. What is Redux? What problem does it solve?
16. What are the three principles of Redux?
17. What is the Redux data flow?
18. What is a Redux store?
19. What is an action in Redux?
20. What is a reducer in Redux?
21. What is dispatch?
22. What is a selector in Redux?
23. What is Redux middleware? Give examples.
24. What is Redux Thunk?
25. What is the difference between Redux and Context API?
26. What is Redux Toolkit (RTK)? How does it simplify Redux?
27. What is `createSlice` in RTK?
28. What is `createAsyncThunk`?
29. What is Redux DevTools?
30. What is immutability in Redux? Why is it important?

### 📋 Interview Questions — Zustand

31. What is Zustand? How is it different from Redux?
32. How do you create a store in Zustand?
33. What is the difference between Zustand and Context API?
34. How does Zustand handle subscriptions and re-renders?
35. What are the advantages of Zustand over Redux?
36. How do you persist state in Zustand?
37. How do you use middleware in Zustand?
38. Can you use Zustand with React Server Components?

### 📋 Interview Questions — React Query / TanStack Query

39. What is React Query? What problem does it solve?
40. What is the difference between server state and client state?
41. How does React Query handle caching?
42. What is stale time in React Query?
43. What is garbage collection time (gcTime) in React Query?
44. What are queries and mutations in React Query?
45. How does React Query handle background refetching?
46. What is optimistic updates in React Query?
47. How is React Query different from Redux for API data?

### 🎯 Scenario Based Questions

48. You have user authentication state needed in 15+ components. What state management would you choose?
49. You have a shopping cart feature. How would you manage the cart state?
50. Your app fetches data from 20 different API endpoints. How would you manage server state?
51. You need real-time updates from a WebSocket. How would you integrate it with your state management?

---

## 3.9 Props

### ✅ Important Topics

- [ ] Passing props
- [ ] Destructuring props
- [ ] Default props
- [ ] PropTypes
- [ ] TypeScript with props
- [ ] Render props
- [ ] Children as props
- [ ] Spread props
- [ ] Callback props
- [ ] Props immutability

### 📋 Interview Questions

1. What are props in React?
2. What is the difference between state and props?
3. Are props immutable? Why?
4. How do you pass data from parent to child?
5. How do you pass data from child to parent?
6. What are default props?
7. What is PropTypes? How do you use it?
8. What is the `children` prop?
9. How do you pass all props to a child component?
10. What is prop spreading? What are its pros and cons?
11. Can you pass functions as props?
12. What is the difference between passing `onClick={handleClick}` and `onClick={() => handleClick()}`?
13. How do you type-check props in React?

---

## 3.10 React.memo, useMemo, useCallback

### ✅ Important Topics

- [ ] React.memo (memoizing components)
- [ ] useMemo (memoizing computed values)
- [ ] useCallback (memoizing functions)
- [ ] Referential equality
- [ ] When to use and when NOT to use
- [ ] Premature optimization
- [ ] Shallow comparison

### 📋 Interview Questions

1. What is `React.memo`? How does it work?
2. What is the difference between `React.memo` and `useMemo`?
3. What is the difference between `useMemo` and `useCallback`?
4. What is referential equality? Why does it matter in React?
5. When should you use `React.memo`?
6. When should you NOT use `React.memo`?
7. Does `React.memo` do a deep comparison?
8. How do you provide a custom comparison function to `React.memo`?
9. What is premature optimization? How does it relate to memoization?
10. Can you memoize a component that receives `children` as a prop?

### 🖥️ Behavior Based Questions

11. Component A passes an inline object `style={{ color: 'red' }}` to a `React.memo`-wrapped child. Will the child re-render on every parent render? Why?
12. You wrap a component with `React.memo` but it still re-renders. What could be the reason?
13. You use `useCallback` for an event handler but the child still re-renders. What's missing?

### 💻 Coding Questions

14. Optimize a list component where each item re-renders when any item changes.
15. Create a component that only re-renders when specific props change.
16. Demonstrate the difference between memoized and non-memoized computation.

---

## 3.11 Lazy Loading & Suspense

### ✅ Important Topics

- [ ] React.lazy()
- [ ] Dynamic import
- [ ] Code splitting
- [ ] Suspense component
- [ ] Fallback UI
- [ ] Route-based code splitting
- [ ] Component-based code splitting
- [ ] Suspense for data fetching
- [ ] Suspense boundaries

### 📋 Interview Questions

1. What is lazy loading in React?
2. What is `React.lazy()`? How does it work?
3. What is code splitting? Why is it important?
4. What is `Suspense`? What is the `fallback` prop?
5. How do you implement route-based code splitting?
6. Can you use `React.lazy` with named exports?
7. What happens if the lazy-loaded component fails to load?
8. Can you nest Suspense boundaries?
9. What is Suspense for data fetching?
10. How does lazy loading improve performance?

### 💻 Coding Questions

11. Implement route-based code splitting with React.lazy and Suspense.
12. Add an Error Boundary around a Suspense boundary for error handling.

---

## 3.12 Error Boundaries

### ✅ Important Topics

- [ ] Error Boundary concept
- [ ] componentDidCatch
- [ ] getDerivedStateFromError
- [ ] Error Boundary limitations
- [ ] Fallback UI
- [ ] react-error-boundary library

### 📋 Interview Questions

1. What is an Error Boundary?
2. How do you create an Error Boundary?
3. Can functional components be Error Boundaries?
4. What errors do Error Boundaries NOT catch?
5. What is `componentDidCatch`?
6. What is `getDerivedStateFromError`?
7. Where should you place Error Boundaries in your component tree?
8. What is the `react-error-boundary` library?
9. How do you recover from an error caught by an Error Boundary?
10. Can you have multiple Error Boundaries in one app?

### 💻 Coding Questions

11. Create an Error Boundary component from scratch.
12. Implement an Error Boundary with a retry button.
13. Add Error Boundaries to a route-level component tree.

---

## 3.13 Performance Optimization

### ✅ Important Topics

- [ ] Identifying performance issues (React DevTools Profiler)
- [ ] Reducing re-renders
- [ ] React.memo, useMemo, useCallback
- [ ] Virtualization (react-window, react-virtualized)
- [ ] Code splitting and lazy loading
- [ ] Debouncing and throttling
- [ ] Avoiding inline object/function creation
- [ ] Key usage in lists
- [ ] Image optimization
- [ ] Bundle size optimization
- [ ] Tree shaking
- [ ] Webpack/Vite optimization

### 📋 Interview Questions

1. How do you identify performance bottlenecks in a React application?
2. What is the React DevTools Profiler? How do you use it?
3. What causes unnecessary re-renders? How do you prevent them?
4. What is virtualization? When would you use it?
5. How does code splitting improve performance?
6. How do you optimize large lists in React?
7. What is the impact of inline functions on performance?
8. How do you reduce the bundle size of a React application?
9. What is tree shaking? How does it relate to React?
10. How does the `key` prop affect list rendering performance?
11. What is windowing/virtualization?
12. How do you optimize images in a React application?
13. What is the difference between `useTransition` and `useDeferredValue`?
14. How does `startTransition` help with performance?

### 🎯 Scenario Based Questions

15. You have a table with 10,000 rows. How do you make it performant?
16. Your app's initial load time is 8 seconds. How do you reduce it?
17. A search input causes the entire app to lag when typing. How do you fix it?
18. Your React app freezes when rendering a complex chart. What do you do?
19. The bundle size of your React app is 5MB. How do you reduce it?

---

## 3.14 Forms in React

### ✅ Important Topics

- [ ] Controlled components
- [ ] Uncontrolled components
- [ ] Form handling with useState
- [ ] Form handling with useReducer
- [ ] Form libraries (React Hook Form, Formik)
- [ ] Form validation
- [ ] File uploads
- [ ] Multi-step forms

### 📋 Interview Questions

1. What is a controlled component?
2. What is an uncontrolled component?
3. What is the difference between controlled and uncontrolled components?
4. When would you use an uncontrolled component?
5. How do you handle form submission in React?
6. How do you handle multiple form inputs with one handler?
7. What is `React Hook Form`? What are its advantages?
8. What is `Formik`?
9. How do you implement form validation in React?
10. How do you handle file uploads in React?
11. What is the `ref` approach for forms? When is it useful?
12. How do you reset a form in React?

### 💻 Coding Questions

13. Build a login form with validation (controlled components).
14. Build a multi-step form with state management.
15. Build a dynamic form that adds/removes fields.
16. Implement form validation without a library.

---

## 3.15 React Router

### ✅ Important Topics

- [ ] BrowserRouter vs HashRouter
- [ ] Routes, Route, Link, NavLink
- [ ] Dynamic routes (useParams)
- [ ] Nested routes
- [ ] Programmatic navigation (useNavigate)
- [ ] Route guards / Protected routes
- [ ] Lazy loading routes
- [ ] 404 page
- [ ] Search params (useSearchParams)
- [ ] Route loaders and actions (React Router v6.4+)
- [ ] Outlet component

### 📋 Interview Questions

1. What is React Router? Why is it needed?
2. What is the difference between `BrowserRouter` and `HashRouter`?
3. What is the difference between `Link` and `NavLink`?
4. What is the difference between `Link` and `<a>` tag?
5. How do you create dynamic routes?
6. What is `useParams`? How do you use it?
7. What is `useNavigate`? How is it different from `useHistory`?
8. What are nested routes? How do you implement them?
9. What is the `Outlet` component?
10. How do you implement protected routes?
11. How do you handle 404 pages in React Router?
12. What is `useSearchParams`?
13. What is `useLocation`?
14. How do you implement route-based code splitting?
15. What are loaders and actions in React Router v6.4+?
16. What is the difference between declarative and programmatic navigation?

### 💻 Coding Questions

17. Implement a Protected Route component that redirects to login if not authenticated.
18. Create a layout with nested routes using Outlet.
19. Implement breadcrumbs based on the current route.
20. Create a 404 page with React Router.

---

## 3.16 Authentication in React

### ✅ Important Topics

- [ ] JWT-based authentication flow
- [ ] Login/Logout flow
- [ ] Token storage (localStorage, cookies, memory)
- [ ] Protected routes
- [ ] Auth context
- [ ] Refresh tokens
- [ ] Axios interceptors for auth
- [ ] OAuth flow in React
- [ ] Role-based access control (RBAC)
- [ ] Session management

### 📋 Interview Questions

1. How do you implement authentication in a React application?
2. Where should you store JWT tokens? What are the tradeoffs?
3. Why is storing JWT in `localStorage` considered insecure?
4. How do you implement protected routes?
5. How do you handle token expiration?
6. What is a refresh token flow? How do you implement it?
7. How do you use Axios interceptors for authentication?
8. How do you implement role-based access control in React?
9. What is the Auth Context pattern?
10. How do you handle "remember me" functionality?
11. How do you prevent authenticated users from accessing the login page?
12. What happens when a user's session expires while they're filling out a form?

### 🎯 Scenario Based Questions

13. A user is authenticated, but their token expires while they're actively using the app. How do you handle this gracefully?
14. You need to implement Google OAuth in your React app. What is the flow?
15. Your app has admin and regular user roles. How do you conditionally render UI based on roles?

---

## 3.17 React Architecture & Best Practices

### ✅ Important Topics

- [ ] Folder structure patterns
- [ ] Feature-based architecture
- [ ] Atomic design
- [ ] Component design principles
- [ ] Separation of concerns
- [ ] Container/Presentational pattern
- [ ] Custom hooks for logic
- [ ] Constants and configuration
- [ ] Environment variables
- [ ] Error handling patterns
- [ ] Code organization best practices

### 📋 Interview Questions

1. What is a good folder structure for a React project?
2. What is feature-based architecture?
3. What is Atomic Design?
4. What is the Container/Presentational component pattern?
5. How do you organize your React project for scalability?
6. Where should you keep API calls in your React project?
7. How do you handle environment variables in React?
8. What are the best practices for writing React components?
9. How do you handle constants and configuration?
10. What is the separation of concerns principle in React?
11. How do you structure a large-scale React application?
12. What naming conventions do you follow for components and files?

### 🎯 Scenario Based Questions

13. You're starting a new React project with 50+ pages. How would you structure it?
14. Your team has 10 developers working on the same React app. How do you prevent conflicts?
15. You need to add a new feature module to an existing React app. How do you organize it?

---

## 3.18 Advanced React Patterns

### ✅ Important Topics

- [ ] HOC (Higher-Order Components)
- [ ] Render Props
- [ ] Compound Components
- [ ] Controlled vs Uncontrolled pattern
- [ ] State Reducer pattern
- [ ] Provider pattern
- [ ] Custom hooks pattern
- [ ] Slots pattern (children manipulation)
- [ ] Inversion of Control

### 📋 Interview Questions

1. What are React design patterns? Name the ones you know.
2. When would you use the HOC pattern vs custom hooks?
3. What is the State Reducer pattern?
4. What is the Provider pattern?
5. What is Inversion of Control in React components?
6. How do you implement a headless component?
7. What is the Compound Components pattern? When is it useful?
8. What is the difference between HOC and custom hooks for code reuse?

### 💻 Coding Questions

9. Build a HOC for authentication checking.
10. Implement the Provider pattern for theme management.
11. Create a Compound Component for an Accordion.
12. Implement a custom hook that replaces a HOC.
13. Build a headless Dropdown component.

---

## 3.19 React Testing (Awareness)

### ✅ Important Topics

- [ ] Unit testing with Jest
- [ ] Component testing with React Testing Library
- [ ] Integration testing
- [ ] Snapshot testing
- [ ] Mocking
- [ ] Testing hooks
- [ ] Testing async components
- [ ] Testing user interactions

### 📋 Interview Questions

1. How do you test React components?
2. What is React Testing Library? How is it different from Enzyme?
3. What is snapshot testing?
4. How do you test a component that makes API calls?
5. How do you test custom hooks?
6. What is the difference between `getByRole`, `getByText`, and `getByTestId`?
7. How do you test user interactions (clicks, form submissions)?
8. What is mocking? How do you mock API calls in tests?
9. What is the testing philosophy of React Testing Library?
10. How do you test error boundaries?

---

## 3.20 React with TypeScript (Awareness)

### ✅ Important Topics

- [ ] Typing props
- [ ] Typing state
- [ ] Typing hooks
- [ ] Typing events
- [ ] Typing refs
- [ ] Generic components
- [ ] Utility types (Partial, Required, Pick, Omit)
- [ ] Interface vs Type

### 📋 Interview Questions

1. How do you type props in React with TypeScript?
2. How do you type the `useState` hook?
3. How do you type event handlers in React?
4. What is the difference between `interface` and `type` for component props?
5. How do you type `useRef` for DOM elements?
6. How do you type the `children` prop?
7. How do you create a generic component in React with TypeScript?
8. How do you type context values?
9. What is `React.FC`? Should you use it?
10. How do you type a component that accepts both specific props and HTML attributes?

---

### 🎯 What Interviewer Expects (React)

- [ ] Deep understanding of hooks (useState, useEffect, useRef, useMemo, useCallback)
- [ ] Understanding of when and why components re-render
- [ ] Knowledge of state management (Context API, Redux/Zustand, React Query)
- [ ] Ability to build custom hooks
- [ ] Understanding of performance optimization techniques
- [ ] Knowledge of React Router and protected routes
- [ ] Understanding of React patterns (HOC, Render Props, Compound Components)
- [ ] Awareness of testing approaches
- [ ] Clean component architecture and folder structure
- [ ] Understanding of React 18+ features

### ❌ Common Mistakes (React)

- [ ] Mutating state directly (e.g., `state.push(item)`)
- [ ] Missing dependency in useEffect dependency array
- [ ] Using index as key in dynamic lists
- [ ] Not handling cleanup in useEffect (memory leaks)
- [ ] Overusing Context for everything (performance issues)
- [ ] Over-optimizing with React.memo/useMemo everywhere
- [ ] Not handling loading/error states
- [ ] Putting everything in a single component
- [ ] Using useEffect for derived state
- [ ] Not understanding the difference between controlled and uncontrolled components
- [ ] Calling hooks conditionally
- [ ] Using `async` directly in useEffect
- [ ] Not knowing when to use useReducer vs useState
- [ ] Storing derived state in useState instead of computing it
- [ ] Passing inline objects/arrays as props without memoization

### 🔥 Must Know Concepts (React)

- [ ] React component lifecycle (class + hooks mapping)
- [ ] Virtual DOM and reconciliation algorithm
- [ ] All hooks and their use cases
- [ ] State management strategies (local, global, server)
- [ ] React Router (nested routes, protected routes, lazy loading)
- [ ] Controlled vs Uncontrolled components
- [ ] Error Boundaries
- [ ] Code splitting with React.lazy and Suspense
- [ ] Performance optimization (memo, useMemo, useCallback, virtualization)
- [ ] Custom hooks creation and best practices
- [ ] React 18 features (Concurrent Mode, Automatic Batching, Transitions)
- [ ] Zustand store setup and usage
- [ ] React Query for server state management

---

> **📌 SECTION 3 COMPLETE — React**

---
