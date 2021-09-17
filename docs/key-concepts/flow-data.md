---
layout: default
title: Flow Data
parent: Key Concepts
nav_order: 6
---

# Flow Data

## Table of contents
{: .no_toc .text-delta }
---
API AutoFlow supports many types of data but the most commonly used is HTTP.  Understanding data structure is important because the flow is about applying actions to the received data and constructing the desired response.

Below is what an HTTP Request and Response data look like.  API AutoFlow receives the HTTP Request data -> Manipulate the data using actions -> Sends the HTTP Response data

## Data Passing Through the Flow
We discussed earlier how flows are simply a chain of actions. The data gets passed from one action to another applying changes based on the action’s properties.

The data that goes through the flow is called “Flow transaction data’. More accurately, it is the data that each action receives from the previous action. The action applies changes to the data and passes it along to the next action.  Hence the action chaining takes place.

### Let’s look at the above example.

1. HTTP server receives request (input) data.
2. The data is passed along to the endpoint with the matching path /helloworld
3. The endpoint passes the data to the next action in the flow
4. The data/set action assigns a string value of “Hello World” to a target called “Result“.
Target is similar to a variable in a programming language
5. The next data/set action assigns the “Result” to the “Response Body (output)”

Calling this endpoint returns the value of “Hello World”

## Using the Data
One of the unique features that make API AutoFlow so easy to use is the availability of HTTP data.  The data can be applied directly to the actions.

Apply changes to the flow data by dragging-and-dropping the field in the action’s settings.

In the above example,

1. by applying the Response Body to the action’s Output at-location
2. you are configuring the Action:data/set to store the data in Response Body

In other words, when the flow (endpoint) is executed, the **Response Body** will have the value __‘Hello World’Note: Reminder that the data that’s been displayed is what the action received from the previous component. Once the current action applies the changes, the flow data with the new value is passed to the next component__

## Data Types
There are 8 data types and 3 data references. To change the data type by selecting from the drop-down.

* **Array**: Array type represents a collection of elements
* **Bits**: Binary
* **Boolean**: Boolean type is true or false
* **Empty**: Empty type is the absence of value
* **Binary in Hex**: Hex representation of Binary
* **Number**: Number type represents numeric data
* **String**: String type represents textual data
* **Object**: Object type represents a collection of properties referenced by an identifier
* **Reference**: Pointer to data. Get value from a variable or mock data (refer to data reference)
* **Table**: Get value from table
* **File**: Get value from File

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> Copy, Paste, Delete Data just like with actions.  The feature is useful when applying the same data structure to many different actions.

## Reference Type
To reference data in the flow transaction data.  It can be understood as a “pointer” to the variable.

[R] [S] is the reference or point to the Flow Transaction Data.
In the example below, [R] is referencing or pointing to the request-body. Hence the data received on the request body will be applied to the action.

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> Dynamic reference pointer
>
> The reference can be dynamic.
>
> Example A: This example uses static value firstname to directly reference the data
>
> Example B: This example gets the value from another data-set “sample-field”
