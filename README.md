# Uncommon HTML Error: Incorrect use of getElementsByTagName
This repository demonstrates a common mistake when working with HTML DOM manipulation, specifically using `getElementsByTagName`.

The issue arises from misunderstanding that `getElementsByTagName` returns an HTMLCollection, not a single element.  Therefore, you cannot directly apply CSS styles to it.

The `bug.html` file shows the incorrect implementation, while `bugSolution.html` provides the correct approach.

## How to Reproduce the Error
1. Open `bug.html` in a web browser.
2. Observe that the paragraph text does not change color.

## Solution
The solution involves iterating through the HTMLCollection and applying the style to each element individually, or selecting the element by ID or class if possible.