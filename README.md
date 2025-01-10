# Unexpected Font Size Inheritance in CSS

This repository demonstrates a common yet subtle CSS bug related to unexpected inheritance of the `font-size` property.  The issue arises when a nested element's `font-size` declaration is unexpectedly overridden by an ancestor's `font-size` declaration. 

The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution.

**Problem:** The nested `<p>` element inside the `.container` div should have a `font-size` of `1em`, but it inherits the `2em` `font-size` from its parent. This is a common problem when working with more complex CSS structures.

**Solution:** A common solution is to reset inheritance using `font: initial` or `font: inherit` or being more explicit with selectors.