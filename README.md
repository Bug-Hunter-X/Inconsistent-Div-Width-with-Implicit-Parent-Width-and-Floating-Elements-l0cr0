# Inconsistent Div Width with Implicit Parent Width and Floating Elements

This repository demonstrates a common CSS layout issue related to implicit parent widths and floating elements. The bug occurs because the width of the parent container is not explicitly set, leading to unexpected behavior in certain browsers. The solution involves setting an explicit width for the parent container, ensuring consistent layout across different browsers.

## Bug

The bug is demonstrated in `bug.css`.  The CSS tries to make two divs each take up 50% of the parent container's width using `float: left;`. However, without an explicit width on the parent, the result is inconsistent across different browsers.  Some browsers might collapse the parent to the minimum width of the floated divs, while others may behave differently.

## Solution

The solution, shown in `bugSolution.css`, simply adds an explicit width to the parent container (e.g., `width: 100%;` or a specific pixel value). This removes the ambiguity and ensures consistent layout.