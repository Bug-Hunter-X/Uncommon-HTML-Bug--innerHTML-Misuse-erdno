# Uncommon HTML Bug: innerHTML Misuse

This repository demonstrates a subtle bug related to the use of `innerHTML` in HTML.  The bug arises from modifying the DOM with `innerHTML` in a way that unexpectedly removes elements that are then referenced.

## Bug Description

The `bug.html` file contains a simple HTML page. The JavaScript code attempts to modify the content of a div using `innerHTML`. However, the second `innerHTML` assignment attempts to modify the original div which is replaced during the first `innerHTML` assignment. This will lead to an unexpected behavior as the second modification has no effect.

## Solution

The `bugSolution.html` file shows the correct approach to solving this issue. It is more robust and prevents accidental modification of non-existent elements.