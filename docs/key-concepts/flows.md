---
layout: default
title: Flows
parent: Key Concepts
nav_order: 3
---

# Flows
Flow is a “service” a developer creates in API AutoFlow to provide certain functionality.

## What is a service?
According to Wikipedia “a service refers to a software functionality (such as the retrieval of specified information or the execution of a set of operations) with a purpose that different clients can reuse for different purposes, together with the policies that should control its usage (For example, based on the identity of the client requesting the service)”

## Action Chaining
Creating a flow is about daisy “chaining actions”.  The actions alter the data to reach the desired result.

![API AutoFlow Action Chainingß](/assets/images/key-points-action-chaining.png)

**[A]** The flow receives a “Request” data

**[B]** The chain of actions makes a change to the data based on the settings

**[C]** The data is sent back as a “Response”
