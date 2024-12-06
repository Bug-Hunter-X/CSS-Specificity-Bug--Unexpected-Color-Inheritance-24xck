# CSS Specificity Bug: Unexpected Color Inheritance

This repository demonstrates a common CSS specificity issue where unexpected color inheritance occurs in nested elements due to the order of declaration in the stylesheet.

The `bug.css` file contains the problematic CSS code, and `bugSolution.css` provides a solution by adjusting the specificity rules.  This bug highlights the importance of understanding CSS specificity when working with nested elements and complex stylesheets. 

## Bug Description
The bug arises from the order of the CSS rules. The more specific selector (`div p`) should logically override the less specific selector (`p`), but due to declaration order, the `color: red` declaration takes precedence, resulting in unexpected output.

## Solution
The solution demonstrates how to resolve this specificity issue by ensuring the more specific rule is defined later or with a higher specificity.