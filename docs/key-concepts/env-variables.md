---
layout: default
title: Environment (Global) Variable
parent: Key Concepts
nav_order: 9
---
# Environment (Global) Variable
A global variable that can be reused throughout the solution.  The environment variable is commonly used to store id, password, IP address, database schema, and more.

## Secret mode
Enables the value to be masked.

## Accessing the data
Use action [data/get-variable](https://docs.apiautoflow.com/docs/actions/data/get-variable/) to access the data.

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips
Use Object or Array data type to store multiple values in the environment variable. If only a String data type is used to store a single value, multiple data/get-variable actions need to be used to access the individual value.
