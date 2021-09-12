---
layout: default
title: Servers
parent: Flow
grand_parent: Overview
nav_order: 1
---

# Servers
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---
This section is a “List view” of the servers created in the solution. When many servers are used, it can be difficult to go from one server to another in the “Solution Section”.  

One of the unique features of API AutoFlow is that there are no limits in the number of servers that can be created. The only limitation is the number of ports available.

## Server Start & Stop

[A] Servers managed from this section. They can be turned on and off, renamed, and deleted.

## Tips

## Status indicators
 Green color indicates that the services are up and working correctly

 Grey color indicates the service is turned off

 Red color indicates that there’s an error. For example, conflict port number

## Server Settings


## Port Number
A number representing a communication endpoint.
There are 65,535 port numbers to choose from.

## Base path
A prefix to apply to every path.
A Base Path + Endpoint Path = Full Path
For example

```
/api/v1 + /resouce = /api/v1/resource
```

## TLS
Formerly known as SSL, TLS is an encryption protocol used to enable HTTPS service

## Access Control
Response header indicates whether the response can be shared with requesting code from the given method, origin, and header

## Tips

## Reserved port numbers
There are reserved port numbers that can not be used. Refer to commonly made mistakes for details.
