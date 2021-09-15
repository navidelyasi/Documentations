---
layout: default
title: Iteration forEach
parent: Iteration
grand_parent: Actions
---
# Iteration forEach
forEach iterates over an array.
in each iteration applies one element of array (as value) to the actions whithin the iteration.

## Properties
```yaml
array: The location of an array that you are iterating over
```

## Output
```yaml
index-location: The location each index is stored
value-location: The location each value is stored
```

This is similar to forEach in Javascript.

Javascript example
```js
var fruits = ["apple", "orange", "cherry"];
fruits.forEach(myFunction);

function myFunction(value, index) {
document.getElementById("demo").innerHTML += index + ":" + value + "<br>";
}
```
**List-target**:  Array fruits
**Value-target**:  Parameter value
**Index-target**:  Parameter index
And the myFunction is the same as the action that goes inside the forEach action.

#### Another example
Let’s say we want to iterate over an array [“a”, “b”, “c”] and capitalize each value.
Using the Testing feature, let’s send an array of [“a”, “b”, “c”] in the request body
Add an Iteration Map Action and assign where you want to read the array from (list-target) and where you want to put the resulting value (value-target)
The action that we want to iterate is first to capitalize the letters, so we will use the action String Capitalize
Finally, we need to set the data in the response body to visualize it on the browser.Let’s read from the data element “iterate” and put it in the “response body”
Below we see that the values in the array have been capitalized
