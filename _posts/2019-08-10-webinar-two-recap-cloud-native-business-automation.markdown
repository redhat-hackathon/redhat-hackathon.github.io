---
layout: post
title:  "Webinar #2 Recap: Cloud Native Business Automation"
date:   2019-10-08
---

In this webinar we covered the **Red Hat Business Automation** stack, which is comprised of **Red Hat Process Automation Manager** and **Red Hat Decision Manager**. We’ve looked at how these platforms can be leveraged in cloud native architectures, providing “process management”, “decisioning” and “rules execution” capabilities to your microservices toolkit.

We recorded the webinar and you can take a look at it [here](https://bluejeans.com/s/vSiSv). The slides are available [here](https://docs.google.com/presentation/d/1MMCqfDQHjCdQsxWA96hJJN523FaBfx_6a10MaXCJ1dg/). For more details and documentation check the [resources section](https://redhat.devpost.com/details/resources) on our [hackathon portal](https://redhat.devpost.com/).

The following illustration shows the various components and capabilities of the Business Automation portfolio.

<center><img src="{{ '/assets/img/red_hat_cloud_native_business_automation.png' | prepend: site.baseurl }}" alt=""></center>

The tools are categorised into **Red Hat Decision Manager (RHDM)** and **Red Hat Process Automation Manager (RHPAM)**. Both these products can be run on bare-metal, Virtual Machines and Cloud (e.g. Red Hat OpenShift).

In this webinar we looked at a number of different topics:

 1. The role of process, rules and decision automation in cloud-native, distributed architectures. We outlined how these business automation capabilities can enhance your cloud-native toolbox.
 2. The high-level architecture of RHDM and RHPAM, introducing the various components like Business Central and the Execution Server.
 3. We discussed the “deployment topology” of RHDM and RHPAM, where we explained that we cannot only deploy these capabilities as a microservice, but that these capabilities can also be embedded in existing (Java based) applications/microservices or can be natively integrated in Spring Boot applications.
 4. We showed how the concept of business automation and decisioning has moved from a centralized deployment model to a de-centralized and distributed set of capabilities.
 5. We outlined a number of real-life use-cases in which process automation and decision engines play an important role, like credit card transaction processing and clinical decisioning.
 6. Red Hat provides various examples and demos that can help you get started with this set of products. We showed the [JBoss Demo Central GitHub repository](https://www.github.com/jbossdemocentral) that contains a vast selection of RHDM and RHPAM demos.
 7. Using the [Order IT HW Demo](https://github.com/jbossdemocentral/rhpam7-order-it-hw-demo), we explained the concept of dynamic cases in the context of Spring Boot applications. We showed how process and rules capabilities allow the implementation of long running processes/cases in the context of a microservices architecture. We demonstrated the implementation of the [Saga pattern](https://microservices.io/patterns/data/saga.html) using BPMN2 compensation events, demonstrating that BPMN2 is very well suited to define and execute complex workflow and orchestration logic in complex inter-microservice communication patterns.
 8. We demonstrated a Decisioning Microservice with the Quick Loan Bank Demo, in which we showed how a set of decisions can be exposed as a microservice via a RESTful API and can be consumed by a modern web-application (e.g. AngularJS, ReactJS).
 9. Finally, we showed you can get started quickly with a Spring Boot-based Business Application via the project generator at [https://start.jbpm.org](https://start.jbpm.org)

We’ll bring you more webinars on our tools in the coming weeks.