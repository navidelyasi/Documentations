---
layout: default
title: Part 4 Update API
parent: Getting Started
nav_order: 4
---

# Part 4: Update API
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }
---
Making update to API AutoFlow is as simple as change the action settings. Which is a good news considering the industry average for software maintenance is around 60% of the total cost.

Let’s say your customer wants to change the date format

2021/04/19  ------>   2021-04-19 -----> 20210419
Making the change
Simply go the String/replace action and remove the “-” in the replacement setting


Result
Now the
 2021-04-19
will change to
20210419

Best Practice
Making changes directly on the “production” can be dangerous. Recommended way of making update is to develop on a “stage” environment and perform enough tests before applying on the production.

How to apply the changes
Best way to apply change is to download the configuration from the development version and upload that on the product.

download config
Tips

Before uploading the new configuration, download the existing configuration from the production to perform rollback if anything goes wrong.
