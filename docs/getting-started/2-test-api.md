---
layout: default
title: Part 2 Test the APIs created
parent: Getting Started
nav_order: 2
---
# Part 2: Test the APIs created
There are several ways to test the APIs you created.

1. Testing using Web browser
2. External Tools: API Testing tools such as Postman.
2. Internal Tools: Built-in Data Simulation and Mock Data

## 1. Testing using Web browser
Since the solution we created in Part One was an HTTP server, we can test the solution using a browser.

Go to `http://api.apiautoflow.com/{your-id}/{your-server-name}/{your-endpoint-name}`.

You can also find the server URL by selecting the server box.

![Data Simulation](/assets/images/getting-started-test-api.png)

Next go ahead and open the browser and navigate to your solution URL.

![Data Simulation](/assets/images/getting-started-test-api1.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/> Tips

> URLs are case sensitive. So `test` is different to `Test`.

## 2. External Tools
There are many API Testing tools such as Postman.
The APIs you created can also be tested using API testing tools such as Postman. One of the advantage of using external tool is that you can send data to the APIs.

![Postman](/assets/images/postman_demo.png)

## 3. Internal Testing
API AutoFlow provides data simulation features to test your solution as you are building it. Data simulation can be enabled by turning the Dev Mode to `ON`.

![Developer Mode](/assets/images/dev-mode-toggle.png)


We will go more in details in the <a href="" alt="">Key Concept</a> section of the documentation, but at a high-level you have the ability to simulate the HTTP Request data **[A]**, then use the data in the actions **[B]**, and see the resulting HTTP response data **[C]** of the solution.

![Data Simulation](/assets/images/data-simulation.png)
