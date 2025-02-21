# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle bug related to the use of `innerHTML` in HTML.  The bug arises from attempting to assign a JavaScript object directly to `innerHTML` instead of a string. This can lead to unexpected behavior, as `innerHTML` expects a string representation of the HTML content.

## The Bug

The `bug.html` file contains the buggy code.  The script attempts to assign a JavaScript object to `innerHTML`, resulting in an empty div.

## The Solution

The `bugSolution.html` file provides a corrected version of the code. The JavaScript object is converted to a string using `JSON.stringify()` before being assigned to `innerHTML`.  Alternatively, you would typically construct the HTML string manually. 

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe the unexpected behavior (empty div).
4. Open `bugSolution.html` and observe the corrected output.