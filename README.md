# Uncommon HTML Bug: Incorrect Display Style in JavaScript Toggle

This repository demonstrates a subtle bug related to toggling the visibility of an HTML element using JavaScript.  The issue lies in the way the `display` style property is handled within the toggle function.

## The Bug

The original code attempts to hide and show a div element using JavaScript. However, it incorrectly sets the `display` style to `null` when attempting to hide the element. This causes unexpected behavior, as `null` is not a valid value for the `display` property.

## The Solution

The corrected code uses the appropriate values for the `display` style:  `"none"` to hide the element and `"block"` to show it.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Click the "Toggle Visibility" button.  Observe the unexpected behavior (element may not hide correctly).
4. Open `bugSolution.html`. Note the corrected code, and see the expected behavior.