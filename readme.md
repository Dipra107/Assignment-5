Dipra Sarker

Assignment 5 Question and Answer


Answering the following questions clearly:


Q1: What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Answer: The difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll is :

The key difference lies in what each method selects and how they return the selected elements.
•	getElementById(id) – Selects a single element by its unique ID. Returns one element or null.
•	getElementsByClassName(className) – Selects all elements with the same class. Returns a live HTMLCollection.
•	querySelector(selector) – Selects the first element matching a CSS selector (e.g., .class, #id, div p). Returns one element or null.
•	querySelectorAll(selector) – Selects all elements matching a CSS selector. Returns a static NodeList (doesn’t update if the DOM changes).
In summary: Use getElementById for unique ID-based selections, getElementsByClassName for live collections of elements by class (though querySelectorAll is often preferred for its static NodeList and broader selector capabilities), and querySelector/querySelectorAll for versatile selections using CSS selectors.


Q2: How do you create and insert a new element into the DOM?

Answer: Creating and inserting a new element into the DOM happens in three main steps:
1. Create the Element
The first step is to create a new, detached element using the document.createElement() method.
2. Set its properties or attributes 
After creating the element,now need to define it’s text, add classes, IDs, or other attributes
3. Insert the Element into the DOM
Finally, Once the element is ready,  need to select a parent element to attach it to. Methods like document.getElementById() or document.querySelector() to get a reference to the parent. Then, use one of the following methods to insert the new element.
-> element.appendChild()
-> element.insertBefore()
-> element prepend()

Q3: What is Event Bubbling and how does it work?

Answer: Event Bubbling is a way events propagate in the DOM. When an event occurs on an element, it first triggers on that element and then bubbles up to its parent elements, all the way to the html element, unless stopped.
It works :
•	Event Trigger: A user action (like a click) occurs on a DOM element (the target).
•	Target Phase: The event is first handled by the element where it occurred.
•	Bubbling Phase: The event moves upward to the parent, then grandparent, and so on.
•	Ancestor Handling: Any parent element with a listener for that event type will also respond.
•	Reaching the Root: The event continues bubbling until it reaches the root of the document (<html>).


Q4: What is Event Delegation in JavaScript? Why is it useful?

Answer:  Event Delegation is a technique in JavaScript for handling events . Where a single event listener is attached to a parent element to handle events triggered by its child elements.
Instead of adding listeners to each child, the parent captures events from its descendants and determines which child triggered the event using event.target.
 It Works:
•	Attach an event listener to the parent element.
•	When a child element triggers the event, the parent’s listener detects the target via event.target.
•	Execute the corresponding action based on the child element.
It’s Useful because :
•	Reduces the number of listeners, improving performance.
•	Works for dynamic elements added after the page loads.
•	Keeps code centralized and cleaner, making maintenance easier.


Q5: What is the difference between preventDefault() and stopPropagation() methods?

Answer: The preventDefault() and stopPropagation() methods serve different purposes in event handling.
preventDefault() stops the browser from doing its usual action - like stopping a link from navigating or a form from submitting. On the other hand, stopPropagation() stops the event from traveling up (or down) the DOM, so parent elements won’t react to it. The key difference is that preventDefault() affects what the browser does by default, while stopPropagation() affects how the event moves through the DOM.


Thank you ……….
