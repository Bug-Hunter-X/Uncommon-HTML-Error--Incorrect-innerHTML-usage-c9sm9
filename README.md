# Uncommon HTML Error: Incorrect innerHTML Usage

This repository demonstrates an uncommon error in HTML related to the usage of `innerHTML`.  The error arises from attempting to set the `innerHTML` property of an element to a JavaScript object instead of a string. This typically results in the object being implicitly converted to '[object Object]', rather than the desired content.

## Bug
The bug lies in the use of `document.getElementById("myDiv").innerHTML = { message: "Hello, world!" };`.

## Solution
The solution involves correctly converting the object to a string representation before setting the `innerHTML`.

## How to reproduce:
1. Clone this repository.
2. Open `bug.html` in a web browser.  You will see that the text is not replaced correctly. 
3. Open `bugSolution.html` to see the corrected code.