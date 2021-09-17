---
layout: default
title: Data Simulation (HTTP)
parent: Data Simulation
grand_parent: Key Concepts
nav_order: 1
---

# Navigation
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---
Flow Test Simulation feature of API AutoFlow enables you to mock the HTTP Request data.

## Response from the Communication Action
The actions that expect a response from another server can mock expected results.

The mock result feature can be turned on and off by clicking the check box .

The simulated mock data in  are made available in the next action as “mock data” in .   

![Data Simulation Action](/assets/images/data-simulation-action.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

1. Start with the mock-result ON to avoid making unwanted calls to the server
Note: under dev mode, flow is executed every time you click on an action
2. Use real data as mock data
After you have configured the action, switch the mock data OFF .  The received data will appear in the next action .  Cut and paste the data back into the action’s mock data.

![Data Simulation Action](/assets/images/data-simulation-action-flow.png)




<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> Multiple sets of request data can be simulated by pressing the + button.  Ideal for testing the solution on varying requests.
