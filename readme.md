Dipra Sarker 

 Answering the following questions clearly:

 
1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Answer: The difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll is :

-->> getElementById(id)

Selects a single element based on its unique ID attribute.

Always returns only one element or null if the ID doesn’t exist.

Example: document.getElementById('header')

-->> getElementsByClassName(className)

Selects all elements with a given class name.

Returns a live HTMLCollection, meaning if the DOM changes (elements are added or removed with that class), the collection updates automatically.

Example: document.getElementsByClassName('item')

-->> querySelector(selector)

Selects the first element that matches a CSS selector (e.g., .class, #id, div p).

Returns a single element or null.

Example: document.querySelector('.item')

-->> querySelectorAll(selector)

Selects all elements matching the CSS selector.

Returns a static NodeList, which does not automatically update if the DOM changes.

Example: document.querySelectorAll('.item')

2. How do you create and insert a new element into the DOM?
Answer: Creating and inserting a new element into the DOM happens in three main steps:

-->> Create the element – The browser provides a method to create a new element node in memory. At this point, it is not yet visible on the page.

-->> Set its properties or attributes – After creating the element, you can define its text, add classes, IDs, or other attributes so it has the content and style you want.

-->> Insert it into the DOM tree – Finally, you place the element in a specific location within the existing structure. This is done by attaching it to a parent element, either at the beginning, at the end, or before/after another element.

Once these steps are completed, the new element becomes part of the webpage and can interact with other elements, events, and styles.

3. What is Event Bubbling and how does it work?
Answer: 
6. What is Event Delegation in JavaScript? Why is it useful?
7. What is the difference between preventDefault() and stopPropagation() methods?




