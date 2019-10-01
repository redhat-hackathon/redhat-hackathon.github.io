---
layout: post
title:  "Working with the Red Hat Managed Platform"
date:   2019-10-01
---

As a continuation of the blog post on Red Hat Managed Platform, here we will get into the details of how you can, as a participant, take advantage of this Platform and which kind of functionality does it provide to you.

Let’s just start by saying that behind the curtains there is a single OpenShift Container Platform running as a multi-user environment. 

What is added to the standard OpenShift is a navigation application (the Solution Explorer) which allows you to explore the available and pre-configured products easily.

<center><img src="{{ '/assets/img/red_hat_platform_01.png' | prepend: site.baseurl }}" alt=""></center>

You will find this tool on your right once you login. To the left you will find tutorials on how to use some of the tools together to achieve a common integration pattern (and by the way, if you feel inspired, you can contribute with your own walkthrough to our Managed Platform [repo](https://github.com/integr8ly/tutorial-web-app-walkthroughs)).

As you will see when accessing any of the tools listed, you will leverage SSO capabilities, saving you from the need of writing the password multiple times. The other advantage of this Platform is that all tools are pre-configured to easily “speak” with each other.

The role that you have been assigned on the Platform allows you to do much more than just using the pre-configured tools. In particular you can:

 - Monitor and browse projects with the web console
 - Configure and utilize the CLI
 - Generate configurations using templates
 - Manage builds and webhooks
 - Define and trigger deployments
 - Integrate external services (databases, SaaS endpoints).

As you have already been exploring the GUI of the Platform, you might have noticed that under the question mark in the right hand corner, there is a Command Line Tools section. This section contains the instructions on how to allow you to access the platform through the [terminal](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/dev-guide-authentication#cli-authentication). This is important because it enables automation scenarios.

As you can see from the documentation you can write your Application using several frameworks. This [tutorial](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/tutorials) will guide you through the whole process of developing locally and then deploying your Application to OpenShift.

Once the Application is running on the Platform you might want to make it reachable from [outside](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/getting-traffic-into-a-cluster) or you might also want to [consume](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/dev-guide-integrating-external-services) services sitting outside the Platform.

Your Application might also need to use sensitive [information](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/dev-guide-secrets) or might just wait for a set of configuration [parameters](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/dev-guide-configmaps).

Finally advanced concept are also explained, like Advanced deployment [strategies](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/deployments#dev-guide-advanced-deployment-strategies), Application [templates](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/deployments) and how to trigger Builds [automatically](https://access.redhat.com/documentation/en-us/openshift_container_platform/3.11/html/developer_guide/builds#dev-guide-triggering-builds).

In terms of role permission, since this is a multi-user environment, we won’t be giving out administrative rights to the participants. The level of permissions assigned to you should be more than sufficient to build, manage, run and monitor applications and microservices on OpenShift which can revolutionize CX in the coming months!

In case you might want to test locally first how the Application works inside the Platform, I suggest you take a look at [minishift](https://www.okd.io/minishift/).

To give you an idea of what you can do you can try the example here [https://fedoramagazine.org/deploy-a-django-rest-service-on-openshift/](https://fedoramagazine.org/deploy-a-django-rest-service-on-openshift/) either on the Platform or in minishift.

As you might have noticed not all the tools mentioned in the Resource page are available as pre-configured in the Platform. In particular:

**Process Automation Manager** can be easily installed by navigating to Service Catalog.

<center><img src="{{ '/assets/img/red_hat_platform_02.png' | prepend: site.baseurl }}" alt=""></center>

And clicking on Middleware -> Process Automation.

<center><img src="{{ '/assets/img/red_hat_platform_03.png' | prepend: site.baseurl }}" alt=""></center>

Once there you should pick either authoring environment (non-HA) or ephemeral (if you just want to try the product without saving results).
Once on the template page you can follow the instructions [here](https://access.redhat.com/documentation/en-us/red_hat_process_automation_manager/7.4/html/deploying_a_red_hat_process_automation_manager_authoring_environment_on_red_hat_openshift_container_platform/environment-authoring-con#template-deploy-mandatory-authoring-proc).

For **Decision Manager** the process is the same as for Process Automation Manager
Once on the template page you can follow the instructions [here](https://access.redhat.com/documentation/en-us/red_hat_decision_manager/7.4/html/deploying_a_red_hat_decision_manager_authoring_or_managed_server_environment_on_red_hat_openshift_container_platform/environment-authoring-managed-con#template-deploy-mandatory-authoring-proc)

In the case of Data Grid, you will start again by navigating in the GUI to the Service Catalog and then to Middleware -> Analytics & Data

<center><img src="{{ '/assets/img/red_hat_platform_04.png' | prepend: site.baseurl }}" alt=""></center>

Once there you choose either the persistent or ephemeral template (with the same limitation as explained above). 
You can find the meaning of the template parameters [here](https://access.redhat.com/documentation/en-us/red_hat_data_grid/7.3/html/red_hat_data_grid_for_openshift/os_templates#os_templates_rhdg_deploy).

An **SSO** instance is pre-configured but this is read only. In case you want to add Authentication & Authorization capabilities to your Application you can deploy the **Red Hat Single Sign On** template.
Start from Service Catalog and click on the integration tab.

<center><img src="{{ '/assets/img/red_hat_platform_05.png' | prepend: site.baseurl }}" alt=""></center>

You can scroll to the end of the page and you will find the SSO template. I suggest to deploy one of the persistent versions. You can find more info [here](https://access.redhat.com/documentation/en-us/red_hat_single_sign-on/7.2/html/red_hat_single_sign-on_for_openshift/getting_started#deploying_the_rh_sso_for_openshift_image_using_application_template).

In the case of **AMQ Streams**, the installation will be on demand, with a dedicated instance per user.

To conclude, if you are just curious about what you can potentially build with this, you can see it summed up in this short video about [Microservices oriented architecture](https://www.youtube.com/watch?v=SPATMHP-xw8) on OpenShift.
