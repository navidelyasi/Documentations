---
layout: default
title: Data
parent: Key Concepts
nav_order: 7
---

# Data
API AutoFlow supports many types of data but the most commonly used is HTTP.  Understanding data structure is important because the flow is about applying actions to the received data and constructing the desired response.

# HTTP Data structure
Below is what an HTTP Request and Response data look like.  API AutoFlow receives the HTTP Request data -> Manipulate the data using actions -> Sends the HTTP Response data

![API AutoFlow HTTP header](/assets/images/data-simulator-http.png)

## Data flowing between actions
We discussed earlier how flows are simply a chain of actions. The data gets passed from one action to another applying changes based on the action’s properties.
The action receives from the previous action, applies changes to the data and passes to the next action.  Hence the action chaining takes place.

![API AutoFlow Data Flow](/assets/images/data-flow.png)

Let’s look at the above example.

* The HTTP server receives request (input) data.
* The data is passed along to the endpoint with the matching path /helloworld
* The endpoint passes the data to the next action in the flow
* The data/set action assigns a string value of “Hello World” to a target called “Result“.
Target is similar to a variable in a programming language
* The next data/set action assigns the “Result” to the “Response Body (output)”
* Calling this endpoint returns the value of “Hello World”


## Apply data to actions
One of the unique features that make API AutoFlow so easy to use is the availability of HTTP data directly to the actions.

![API AutoFlow Applying Data to Flow](/assets/images/apply-data-to-action.gif)

Apply changes to the action by dragging-and-dropping the data to the action’s settings.

In the above example, by applying the Response Body to the action’s `Output` you are configuring the `Action:data/set` to store the data in `Response Body`.

In other words, when the flow is executed, the Response Body will have the value ‘Hello World’

Note: The data that’s been displayed in the right pane is the data received from the previous action. Once the current action applies the changes, the changed data is passed to the next action.

## Data Referencing
Above use of data in action can be comparable to `Reference` in the programming world or even a “pointer” to a variable.

`[R]` data type is the reference or pointer to the to the data.

In the example below, [R] is referencing or pointing to the request-body. Hence the data received on the request body will be applied to the action.

![API AutoFlow Applying Data Referencing](/assets/images/data-referencing.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> Dynamic reference pointer
>
> The reference can be dynamic.
>
> Example A: This example uses static value firstname to directly reference the data
>
> Example B: This example gets the value from another data-set “sample-field”


![API AutoFlow Applying Data Referencing](/assets/images/data-referencing1.png)



### Let’s look at the above example.

1. HTTP server receives request (input) data.
2. The data is passed along to the endpoint with the matching path /helloworld
3. The endpoint passes the data to the next action in the flow
4. The data/set action assigns a string value of “Hello World” to a target called “Result“.
Target is similar to a variable in a programming language
5. The next data/set action assigns the “Result” to the “Response Body (output)”

Calling this endpoint returns the value of “Hello World”
