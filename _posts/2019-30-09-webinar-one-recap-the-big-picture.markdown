---
layout: post
title:  "Webinar #1 Recap: The big picture: How the Red Hat Open Source stack fits together"
date:   2019-09-30
---

In our first webinar we covered Red Hat’s open source philosophy Hat and how communities create outstanding software. We then zoomed in on the middleware tools that Red Hat offers, how these fit together and how they can be leveraged in the hackathon. 

We recorded the webinar and you can take a look at it [here](https://bluejeans.com/s/deeHS). The slides are available [here](https://speakerdeck.com/manfredbo/the-big-picture-how-the-red-hat-open-source-stack-fits-together). For more details and documentation check the [resources section](https://redhat.devpost.com/details/resources) on our [hackathon portal](https://redhat.devpost.com).

The following illustration shows the various middleware tools and categories summarised. 

<center><img src="{{ '/assets/img/red_hat_open_source_stack.png' | prepend: site.baseurl }}" alt=""></center>

The tools are categorised into Red Hat Application Environments, Red Hat Integration and Red Hat Process Automation. All of those can integrate with and leverage Red Hat Single Sign-on, and all of them are hosted and managed for you on top of the Red Hat container platform OpenShift. 

In the webinar we took a look at each of the tools in more detail to give you an idea about the capabilities and how they can be used. 

 1. Red Hat Application Runtimes for application development: It’s a set of products, tools, and components for developing (cloud-native) applications. It includes lightweight runtimes and frameworks for building cloud- and/or microservice-based architectures (among others Java, Spring, NodeJS, Web, Serverless, Vert.X etc.).
 2. Red Hat Fuse for integration: Fuse is a typical integration technology. It offers a wide range of connectors, integration and transformation patterns. Fuse can be used to build decentralised integration logic or leverage ESB capability.
 3. Red Hat AMQ for messaging: It’s a lightweight, high-performance, event-based messaging platform for enterprise applications. It includes also AMQ Streams (based on Kafka) which offers a distributed messaging backbone. It allows apps, services or microservices to share data with extremely high throughput and extremely low latency.
 4. Red Hat 3scale API Management: It makes it easy to secure and manage REST APIs for internal or external users. 3scale offers capabilities to share, secure, distribute, control, and monetize REST APIs on an infrastructure platform built with a focus on performance and scalability.
 5. Red Hat Process Automation Manager: This tool enables users to document, simulate, manage, automate and monitor business processes and decisions. It supports automation of cloud-native and/or microservice based business applications. 
 6. Red Hat Decision Manager: It offers a fast and lightweight decision management platform. It enables developers and business users to create rules and decision driven applications or services in an agile way. Example use-cases include: credit-scoring, fraud detection, premium calculation and law & regulatory compliance.
 7. Red Hat DataGrid for distributed caching: It’s an in-memory, distributed, NoSQL datastore solution (= distributed cache). DataGrid decreases response times and allows you to improve performance, and increase app availability, reliability, and scale.
 8. Red Hat Single Sign-on (SSO) for application security: It’s based on the Keycloak project. It enables securing Web applications by providing single sign-on (SSO) capabilities. It can be used to leverage popular standards such as SAML 2.0, OpenID Connect and OAuth 2.0. Red Hat SSO can act as an Identity Provider, mediating between apps, user directories or 3rd-party SSO providers for identity information via standards-based tokens.

As a reminder, all these tools are available through an AppDev platform managed by Red Hat, which is based on the very popular container platform OpenShift.  We’ll bring you more webinars on our tools in the coming weeks.
