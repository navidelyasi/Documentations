---
layout: default
title: Part 1 Create a Solution
parent: Getting Started
nav_order: 1
---

# Part 1: Create a Solution

To create your first solution, you first need to create an account on API AutoFlow Cloud.  Press below button to navigate to the cloud console.

[API AutoFlow Cloud](https://console.apiautoflow.com/){: .btn .btn-primary }

Alternatively, you can follow the <a href="" alt="">instructions</a> to download and try the install version.

## Hello World!

The first solution we'll create to together is the good old "Hello World!" solution where you create an API that prints a string value of `"Hello World!"`.

To do that you will start by creating three things on the solution page.
1. Server
2. Endpoint
3. Action

Follow below instructions to create each on your solution page.

## 1. Create Server
Add a HTTP server by selecting the [Add] drop-down on the top of the screen. API AutoFlow supports many different server types, but when using a web based API, most common protocol is HTTP(S).

![Create Server](/assets/images/create_server.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/> Tips

> The server will be created with a random port number. You can change the port number by selecting the Server box which opens the Server settings.
>
> **Change Port Number**
>
> Change the port number to `1111`
>
> ![Port Number](/assets/images/port_number_change.png)

## 2. Create Endpoint
Add a server endpoint by selecting the **[Add]** drop-down on the top of the screen.  

Follow below steps.

![Create Endpoint](/assets/images/create-endpoint.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/> Tips

> The endpoint by default has a root path `/`. You can change the root path to /test.

### Change Path

* Change the path to `/test`
* Change the method to `GET`

![Change Path](/assets/images/change-endpoint-path.png)


## 3. Apply Action

From the right pane, select the **Action** tab and navigate to Data category. From there, drag and drop the `set` action to the flow you just created. When you start dragging the action, you'll see a circle appear at the end of the flow where you can place the action.

![Database Integration](/assets/images/database-integration.gif)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/> Tips

> Actions are categorized based on their functions. You can also use the search feature to quickly find the action you need.  List of all the actions are in the <a href="" alt="">Action</a> section of the documentations.

### Set data output to HTTP Response Body.
Since we are using an HTTP service, we can send respond back in the HTTP Response Body. This will enable us to test the solution on a regular web browser.

Drag and drop the response body from right-bottom pane to the action's output.

![Output](/assets/images/action-output.gif)

Next, let's move over to the next section to learn different ways solutions can be tested.

[NEXT >> Test API](https://docs.apiautoflow.com/docs/getting-started/2-test-api){: .btn .btn-primary }
