# CSS Flexbox Centering Bug

This repository demonstrates an uncommon issue related to centering flex items using `margin: 0 auto;` within a flex container.  The problem arises from the interaction between the `margin` property and the flexbox layout model. While `margin: 0 auto;` effectively centers block-level elements, it behaves unexpectedly with flex items in certain situations.

## The Bug

The `bug.css` file contains CSS code that illustrates the issue.  Notice that even though we're using `justify-content: space-between` and applying `margin: 0 auto;` to the flex items, they don't center as expected. 

## The Solution

The `bugSolution.css` file provides a correct solution using `margin: auto` on the left and right sides, only. This fixes the unexpected behavior and centers the elements properly within the flex container.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` (or create your own HTML using the CSS). 
3. Observe the unexpected centering behavior of the flex items.
4. Replace the CSS with the corrected code from `bugSolution.css` and see the improvement.

This example highlights the importance of understanding the nuances of flexbox layout and how different CSS properties interact within it.