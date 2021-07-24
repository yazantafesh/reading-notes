# AWS: Cloud Servers

## Review, Research, and Discussion

- Describe the Web-Request-Response-Cycle

  It is the cycle that represents how each process will be done when we are using the internet. When we hit http link, this request will go to the server and maybe to database also or other servers, finally will return a response to the client.

- Explain what a “server” is, as it relates to the WRRC.

  A ***server*** is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.

  In the web we interact with a web server, which is a computer program that serves requested HTML pages or files. In this case, a web browser acts as the client. Usually the server interact with a database by the request of the client.

- What does it mean to “deploy” an application?

  Deploying your application means putting it on a Web server so that it can be used either through the Internet or an intranet.

## Document the following Vocabulary Terms

- **Server** is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.

- **Pub/Sub** Publish/Subscribe allows services to communicate asynchronously, with latencies on the order of 100 milliseconds. Pub/Sub is used for streaming analytics and data integration pipelines to ingest and distribute data. It is equally effective as messaging-oriented middleware for service integration or as a queue to parallelize tasks.

- **WRRC** traces how a user’s request flows through the app , it includes the client sending a request to the backend server , the backend server would do some process then send a response back to the client.

## Preparation Materials

### *Virtual Machines*

  This video briefly but effectively explains what a virtual machine is, along with several other terms that make it easier to understand what a virtual machine is and does.

### *VMS and the Cloud*

  - What is ***Virtualization***: Virtualization enables users to disjoint operating systems from the underlying hardware, i.e, users can run multiple operating systems such as Windows, Linux, on a single physical machine at the same time.

  - ***Hypervisor***: A hypervisor, also known as a virtual machine monitor or VMM, is software that creates and runs virtual machines (VMs). A hypervisor allows one host computer to support multiple guest VMs by virtually sharing its resources, such as memory and processing.

  - ***Cloud computing*** : is the on-demand availability of computer system resources, especially data storage (cloud storage) and computing power, without direct active management by the user.

### *AWS EC2*

  Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.

### *Elastic Beanstalk*

  ***AWS Elastic Beanstalk*** is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, and Docker on familiar servers such as Apache HTTP Server, Apache Tomcat, Nginx, Passenger, and IIS. You can simply upload your code and Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring.

