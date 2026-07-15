# React.js


### 1. What is Largest Contentful Paint (LCP)?

* LCP is one of Google’s Core Web Vitals that measures how long it takes for the largest visible element on a page to load.
* A good LCP score indicates that users can view the main content of the page quickly, leading to a better user experience.


### 2. Have you written unit test cases for API calls? How do you test them?

* Yes. API calls are typically tested by mocking the network request and verifying different scenarios such as successful responses, loading states, and error handling.
* This ensures the component behaves correctly without making actual API requests during testing.


### 3. Have you used Jest or Enzyme?

* Jest is commonly used alongside React Testing Library to test components from a user’s perspective, while Enzyme was more popular with older React versions.


### 4. How can data be communicated between two browser tabs?

* Some common approaches include using the BroadcastChannel API, the storage event with localStorage, or SharedWorker, depending on the use case and browser support.
* The interviewer was interested in understanding when each approach would be appropriate.


### 5. What is type casting in TypeScript?

* Type casting allows you to tell TypeScript how a value should be treated when its type cannot be inferred automatically.
* It is commonly done using the as keyword or angle bracket syntax, helping improve type safety while working with dynamic data.

### 6. What is the difference between package.json and package-lock.json?

* package.json contains project metadata, dependencies, and scripts.
* package-lock.json stores the exact versions of all installed dependencies, ensuring consistent installations across environments.

### 7. What is the difference between ^ and ~ in dependency versions?

* ^ allows updates to minor and patch versions.
* ~ allows only patch version updates.

These symbols help manage dependency updates without introducing unexpected changes.

 ### 8.What is the difference between null and undefined?

* undefined indicates that a variable has been declared but not assigned a value.
* null is an intentional assignment that represents the absence of a value.

### 9. JavaScript Output-Based Questions

The interview also included output-based questions to assess understanding of:

* Closures
* Hoisting
* Event Loop
* Variable Scope
* this keyword
* Promise execution order

### 10. How did you improve performance in a slow application?
* Use React.memo to prevent child components from re-rendering when their props hadn't changed.
* Wrapped expensive calculations, such as filtering and transforming data, in useMemo.
* Use useCallback for event handlers passed to memoized child components so they received stable function references.
* Add lazy loading with React.lazy and Suspense for pages that weren't needed during the initial load.
* Reduce unnecessary API calls by debouncing the search input.
* Broke large components into smaller reusable components to reduce the rendering scope.
* Remove unnecessary state updates and ensured immutable state updates.

### 11.Why did you choose React Query over Redux?
I chose React Query because most of the data in my application came from APIs. React Query handles fetching, caching, synchronization, background refetching, loading, and error states out of the box. Redux is better suited for managing global client-side state like user preferences, theme, or sidebar state, but it's not optimized for server state.

### 12. Tell me about a production issue you solved.
Situation: "We received reports from customers that after updating an order's status, the UI still showed the old status until they refreshed the page."

Task: "I was responsible for identifying why the UI wasn't updating correctly and fixing it without introducing regressions."

Action: "I reproduced the issue in the development environment and used Chrome DevTools and React DevTools to inspect the component state and network requests. The API response contained the updated status, so the backend was working correctly. I found that the component was relying on stale local state that wasn't being updated after the API call. I updated the state management so the UI refreshed with the latest data immediately after a successful update. I also tested related workflows to ensure the fix didn't affect other screens."

Result: "The issue was resolved, users no longer needed to refresh the page to see updates, and support tickets related to that problem stopped."

### 13. What trade-offs did you consider while designing a feature?


✅ React Fiber & Reconciliation
✅ Building an Infinite Scrolling component for large API datasets
✅ "useRef" vs "useEffect" and their use cases
✅ Why Promises (Microtasks) execute before "setTimeout" (Macrotasks)
✅ Explain Microservices and  Micro Frontends
✅ Middleware in Express.js
✅ Creating a Express.js server from scratch and add 2 routes.
✅ JavaScript event loop output prediction involving:
- "setTimeout()"
- "setImmediate()"
- "process.nextTick()"

✅ Techniques to improve slow API performance on the server side
✅ What is  Parameterized SQL Queries
 How would you optimize API calls in a React application?

 📌 ReactJS Questions

✅ Controlled vs Uncontrolled Components
✅ Ref Forwarding in React 19
✅ React Portals and their use cases
✅ Lazy Loading and performance optimization
✅ Higher-Order Components (HOCs)
✅ Redux useSelector
✅ React Routing
✅ Handling 404 (Page Not Found) routes

📌 JavaScript Questions

✅ What is Debouncing?
✅ Implement a Debounce function
✅ Spread Operator with examples
✅ Find the First Non-Repeated Character in a string
✅ Hoisting in JavaScript

📌 CSS & Web Concepts

✅ CSS Sprites
✅ How z-index works

📌 API & Performance

✅ Axios Interceptors and their use cases
