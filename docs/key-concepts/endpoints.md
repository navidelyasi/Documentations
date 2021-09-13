---
layout: default
title: Endpoints
parent: Key Concepts
nav_order: 4
---

# Endpoints
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---
An HTTP or API endpoint is basically a fancy word for a URL/URI of a server or service.


## Path
URI path.   `/`  is the root path

## Serve File
Way to host a file such as index.html
See below for more details

## Method
Defines a set of request methods to indicate the desired action to be performed for a given resource.
Most commonly used methods are POST, GET, PUT, PATCH, and DELETE.

## Serve File


**Serve Files** is a means to host the files. You can point to the dist directory generated from frameworks such as Vue.js, Angular, ReactJS, etc

#### For example

* Given a folder:  my-folder/index.html
* An endpoint with path:  /ui

Serve files: my-folder

Then you can open:

```
<protocol>://<address>:<port>/ui/index.html
```

## Body [Canary]

**__Server Endpoint Body is in Canary stage__**

Body applies validation to incoming requests.

It is a JSON Schema.

The future release will have a tighter integration with the Schema.
