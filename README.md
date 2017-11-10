# Design Decision Tool for IaaS on IBM Cloud

The Design Decision Tool contains the potential advantages and disadvantages of the available components used for designing and building your infrastructure as a Service (IaaS) on IBM Cloud.  Use this information during your solution design to help select the best options to meet your workload requirements.  More information is provided in the [IaaS Solutions Design training class] (http://www.softlayer.com/training-courses) which takes you through hands-on workshops to assist you with making architecture choices for your IaaS.

## How to use the Design Decision Tool 

The Design Decision Tool supports the infrastructure process (Figure 1) by stepping you through each component of your infrastructure to help you determine which options to use based on your requirements.  You are encouraged to use the design process and decision tool when designing your IaaS.

![Figure 1: IaaS design process](/images/rainbow_tool_fig1.png)

Figure 1: IaaS design process

A high-level example of an e-commerce workload has been provided to assist you with the Design Decision Tool. After reviewing the example you can then apply the concepts to your workload. 

## Indie Tix, Online Ticket Retailer (e-Commerce Example)

Indie Tix is an online ticket retailer that promotes indie music to mainstream listeners by putting on concerts in intimate venues (500 to 3,500 seats). In their current environment, they are facing increases in demand as indie artists are gaining popularity due to Internet exposure and mainstream air play.

They will be designing an architecture based on three tiers – web, application, and database - based on their current and future needs. The tiers are divided into three layers – presentation (web), business (application), and data (database) – with a server residing in each. Figure 2 illustrates Indie Tix’s architecture.

![Figure 2: Indie Tix's 3-tier architecture design](/images/rainbow_tool_fig2.png)

Figure 2: Indie Tix's 3-tier architecture design

The first component to be determined is the global load balancer, which has the following requirements:

* Available storefront – up to 24x7 – for top-tier customers
* Anticipate traffic spikes that “follow the sun”
* Handle seasonal spikes in service usage
* Support 7,500 unique shoppers daily and 100 connections per second
* Support highly variable and unpredictable compute requirements


![Figure 3: Compute Options](/images/rainbow_tool_compute_options.png)
