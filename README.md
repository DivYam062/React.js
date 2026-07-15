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
