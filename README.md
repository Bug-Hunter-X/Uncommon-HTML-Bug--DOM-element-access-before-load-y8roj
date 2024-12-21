# Uncommon HTML Bug: DOM Element Access Before Load

This repository demonstrates a subtle bug that can occur in HTML when attempting to manipulate the DOM (Document Object Model) before the element has fully loaded.

## The Bug
The bug arises from accessing a DOM element using `document.getElementById()` before the browser has finished parsing and rendering the HTML.  This often results in the element not being manipulated correctly, or in some cases, causing a JavaScript error.

## The Solution
The solution involves using the DOMContentLoaded event listener. This ensures that the code to manipulate the DOM is executed only after the entire HTML document is fully parsed and loaded. 