---
layout: default
title: Data Simulator
parent: Key Concepts
grand_parent: Actions
has_children: true
permalink: /docs/actions/key-concepts/data-simulator
nav_order: 13
---

# Data Simulator
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---

### What is Simulated (Mock) Data?
Mock data is the simulated or made-up data.

What type of data can you mock in the product?

1. HTTP Requests
The process of creating a flow is to design a chain of actions that provides desired response to the request.  By simulating the request data within the product, developers can visualize the expected response as the flow is built and actions are applied.

2. Actions receiving data
Database and communication actions receive data from another server.  During development, it may not be ideal to execute those actions too many times for reasons such as rate limiting and slow responses delaying the development process.
