# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to using innerHTML to modify the CSS `display` property of an HTML element.  The issue arises when trying to change the display style (e.g., to hide an element) using innerHTML instead of directly manipulating the element's style or class.

## Bug Description
The `bug.html` file contains a simple HTML structure with a div element.  Javascript code attempts to hide this div using `innerHTML`. This approach does not correctly change the `display` property.  While the content *appears* to change, the `display` remains unchanged, potentially leading to unexpected behavior, especially if other logic depends on correct visibility.

## Solution
The `bugSolution.html` file provides a corrected version.  The display property is correctly set using either direct style manipulation (recommended) or class manipulation.

## How to reproduce
1. Clone the repository.
2. Open `bug.html` in a web browser.
3. Observe that the div element is still visible despite the attempted hiding via innerHTML.
4. Open `bugSolution.html`. The element is correctly hidden in this solution.