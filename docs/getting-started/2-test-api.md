---
layout: default
title: Part 2 Test the APIs created
parent: Getting Started
nav_order: 2
---

# Part 3: Test the APIs created
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---
There are several ways to test the API.

1. Internal Testing: Built-in Data Simulation and Mock Data
2. External Testing: API Testing tools such as Postman.

## Internal Testing: Data Simulation and Mock Data
### What is Simulated (Mock) Data?
Mock data is the simulated or made-up data.

What type of data can you mock in the product?

1. HTTP Requests
The process of creating a flow is to design a chain of actions that provides desired response to the request.  By simulating the request data within the product, developers can visualize the expected response as the flow is built and actions are applied.

2. Actions receiving data
Database and communication actions receive data from another server.  During development, it may not be ideal to execute those actions too many times for reasons such as rate limiting and slow responses delaying the development process.

## Simulating HTTP Request

![Data Simulation](/assets/images/data-simulation.png)

As discussed earlier on understanding flow creating a flow is all about how you manipulate the HTTP request data to send back the desired HTTP response.

Flow Test Simulation feature of API AutoFlow enables you to mock the HTTP Request data.

The request data simulated in  are made available as “mock data” in .   The expected response gets displaced in .

## Tips

Multiple sets of request data can be simulated by pressing the + button.  Ideal for testing the solution on varying requests.


![Developer Mode](/assets/images/dev-mode-toggle.png)

Data simulation can be enabled by turning the Dev Mode ON or OFF.

## Response from the Communication Action
The actions that expect a response from another server can mock expected results.

The mock result feature can be turned on and off by clicking the check box .

The simulated mock data in  are made available in the next action as “mock data” in .   

![Data Simulation Action](/assets/images/data-simulation-action.png)

## Tips

1. Start with the mock-result ON to avoid making unwanted calls to the server
Note: under dev mode, flow is executed every time you click on an action
2. Use real data as mock data
After you have configured the action, switch the mock data OFF .  The received data will appear in the next action .  Cut and paste the data back into the action’s mock data.

![Data Simulation Action](/assets/images/data-simulation-action-flow.png)

## External Testing: API Testing tools such as Postman
The APIs you created can also be tested using API testing tools such as Postman.
![Postman](/assets/images/postman_demo.png)
