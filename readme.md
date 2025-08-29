1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

 1. getElementById: Finds a single element based on its unique ID.

 2. getElementsByClassName: Retrieves all elements with a given class name, returning an HTMLCollection.

 3. querySelector: Returns the first element that matches a given CSS selector.

 4. querySelectorAll: Returns all elements matching the selector, as a NodeList.


2. How do you create and insert a new element into the DOM?

Ans const newHistory = document.createElement("div"); newHistory.textContent= "Hi"; document.body.appendChild(newHistory);


3. What is Event Bubbling and how does it work?
Ans
Event bubbling is the process where an event triggered on a nested element first runs on the target element and then propagates upward through its ancestors in the DOM tree.
Example: Clicking a button inside a <div> first fires the button’s event, then the <div>’s, then the <body>, and finally the document.


4. What is Event Delegation in JavaScript? Why is it useful?
Event delegation is a technique where a parent element listens for events on its child elements by using event bubbling.
It’s useful for:

 1. Handling events on dynamically created elements.

 2. Reducing memory usage by avoiding multiple event listeners.


5. What is the difference between preventDefault() and stopPropagation() methods?

preventDefault(): Prevents the default browser action (e.g., stopping a form from submitting).

stopPropagation(): Prevents the event from bubbling up to parent elements.
