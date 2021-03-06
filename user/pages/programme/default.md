---
title: Programme
---

<style>
#footer {
   display: none;
   }
</style>

#### ContainerDays Boston 2015

<img src="http://dynamicinfradays.org/events/2015-boston/2015-boston-logo.png" height="241" width="300" style="margin-left:auto;margin-right:auto;display:block">

### Talks

#### <a name="briefhist"></a>_A Brief History of Containers_ <span style="font-size: smaller">- [Jeff Victor](#jeffv) & [Kir Kolyshkin](#kirk)</span>

Containers are a form of operating system virtualization that is subtly different from virtual machines. The concept has evolved over time, and Jeff and Kir will discuss the history of OSV and the roles of current implementations.

slides [1](http://www.slideshare.net/DynamicInfraDays/containerdays-boston-2015-abriefhistoryofcontainers) [2](https://www.slideshare.net/kolyshkin/brief-history-of-linux-containers) [video](https://www.youtube.com/watch?v=doUktZIcXF0)

#### <a name="elbatscale"></a>_Elastic Load Balancing at Scale with Mesos and Docker_ <span style="font-size: smaller">- [Stephen Salinas](#stephens)</span>

The HubSpot product is made up of over 200 separately deployable web APIs. While investing in a Service Oriented Architecture has many benefits, it can also expose new infrastructure scaling challenges.

Stephen will discuss the challenges faced, and how his team built a Mesos-based software load balancer using Docker that improves reliability, decreases human intervention, and saves money.

[slides](http://slides.com/stephensalinas-1/hubspot-container-days-2015)

#### <a name="kubern"></a>_Kubernetes: Container Orchestration at Scale_ <span style="font-size: smaller">- [Max Forbes](#maxf)</span>

Kubernetes is an open source orchestration system for Docker containers. It handles scheduling onto nodes in a compute cluster and actively manages workloads to ensure that their state matches the users' declared intentions.

Max will explain the motivation for Kubernetes and cover Kubernetes core concepts, and why these concepts are useful. He'll spin up a Kubernetes cluster and demonstrate these concepts live by deploying a simple application, as well as touching on what's next for Kubernetes and container orchestration.

[slides](https://speakerdeck.com/mbforbes/kubernetes-container-orchestration-at-scale) [video](https://www.youtube.com/watch?v=x8WiYujLbgc)

#### <a name="sepconcerns"></a>_Implementing Separation of Concerns with Containers_ <span style="font-size: smaller">- [J&eacute;r&ocirc;me Petazzoni](#jeromep)</span>

One of the promises of containers is to offer "separation of concerns" between Devs and Ops. Devs are supposedly able to put their code in containers, run those containers locally, and ship them to the Ops team. When deployed on other platforms (from test to staging to QA to production), those containers will behave exactly the same way as they did in development.

But what should we do when our production platform uses a totally different logging system? How should we implement backups or metrics collection in our production containers, without bloating our development containers? In development, it's easy to use a mechanism like Docker Compose to bring up multiple containers together, but how does that work in production stacks?

J&eacute;r&ocirc;me will present many techniques to answer those questions (and a few more), and show how our application containers can remain simple and lean, yet have all the indispensable bells and whistles that are required
to run in stable production environments.

[slides](http://www.slideshare.net/jpetazzo/implementing-separation-of-concerns-with-docker-and-containers) [video](https://www.youtube.com/watch?v=pUQ5ukrVaH4)

#### <a name="persist"></a>_Containerized Data Persistence on Mesos with Kafka, MySQL, Cassandra, HDFS and More!_ <span style="font-size: smaller">- [Joe Stein](#joes)</span>

Being able to containerize data persistent systems has traditionally been difficult. With the ability to now have data persistent frameworks such as Kafka, MySQL, HDFS, etc. running on Mesos, we not only gain benefits from containerizing but can build out new features we were never able to deliver before.

Joe will talk through where things are today, what to watch out for, and where things are heading moving forward.

[slides](http://www.slideshare.net/mobile/charmalloc/containerized-data-persistence-on-mesos) [video](https://www.youtube.com/watch?v=PEbXWpgQVcU)

#### <a name="lambda"></a>_Thinking Differently: An Introduction to AWS Lambda_ <span style="font-size: smaller">- [Tara Walker](#taraw)</span>

AWS Lambda is a new compute service that runs your code in response to events and automatically and dynamically manages infra resources for you. Tara will talk about AWS's event-driven compute strategy and explain how Lambda works to respond to events from various Amazon services.

Tara will describe what you need to quickly begin building applications that use AWS Lambda as a serverless back-end, and will also cover key Lambda features, its programming model, and tips on getting the most out of Lambda functions.

[slides](http://www.slideshare.net/AmazonWebServices/a-walk-in-the-cloud-with-aws-lambda) [video](https://www.youtube.com/watch?v=giEZuC5NFes)

#### <a name="journey"></a>_Running Docker, Mesos and More in Production: The Journey to Container Adoption in the Enterprise_ <span style="font-size: smaller">- [Igor Moochnick](#igorm)</span>

Enterprises have well-established cultures, technology stacks and processes. Now containers are changing the way we think about applications, artifacts and deployment processes. They also bring new challenges along the way, especially since the technology is still young and constantly changing.

Igor will discuss how this new set of technologies is finding its way in the enterprise, and what we've learned so far.

[slides](http://www.slideshare.net/igor.moochnick/the-journey-to-container-adoption-in-enterprise) [video](https://www.youtube.com/watch?v=QldAEl7X0BE)

#### <a name="layers"></a>_CoreOS: Building the Layers of the Scalable Cluster for Containers_ <span style="font-size: smaller">- [Barak Michener](#barakm)</span>

One of the strengths of containerization is the way it allows us to consider how to build our applications for scale. Turning a cluster of machines into a single, highly-available computer is the end goal of a containerized world.

However, there are many distributed systems problems along the way!

Barak will discuss the layers that tend to constitute a cluster (from the hardware up) and talk about the multiple open-source projects at CoreOS that build these layers through small, composable utilities.

[slides](http://www.slideshare.net/DynamicInfraDays/containerdays-boston-2015-coreos-building-the-layers-of-the-scalable-cluster-for-containers-barak-michener) [video](https://www.youtube.com/watch?v=K7oMynmiA0c)

#### <a name="nproblems"></a>_N Problems of Linux Containers...and Some Solutions_ <span style="font-size: smaller">- [Kir Kolyshkin](#kirk)</span>

The talk gives an insight into some of the core problems brought about by Linux Containers, and how they were solved over the years. While most of these problems and solutions belongs in the Linux kernel, kernel knowledge is not expected from the audience.

Kir will cover:

* Resource management mechanisms (including cgroups, VSwap, I/O and CPU limits and priorities)
* "File system in a file" technology (ploop)
* Approaches for fast live migration (ploop write tracker, CRIU, iterative checkpoint/restore)
* Docker interoperability

[slides](http://www.slideshare.net/kolyshkin/n-problems-of-linux-containers-49400161) [video](https://www.youtube.com/watch?v=bzQeMiruVFg)

#### <a name="cdwithcontainers"></a>_Continuous Delivery with Containers_ <span style="font-size: smaller">- [Nick Gauthier](#nickg)</span>

Automated Continuous Delivery of software applications is the modern way of getting your product in front of users. Having an automated pipeline means you don't have to worry about deploys and lets your software team focus on code and your operations team focus on infrastructure.

Containers take this process to a new level with clean isolation and a clear API between infrastructure and application. In this talk we'll explore how to containerize your application with Docker and how that impacts your Continuous Delivery process.

[slides](http://www.slideshare.net/DynamicInfraDays/containerdays-boston-2015-continuous-delivery-with-containers-nick-gauthier) [video](https://www.youtube.com/watch?v=NgQnR1vhfOY)

### Speakers

<img src="http://dynamicinfradays.org/events/2015-boston/max-forbes.png" width="117" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="maxf"></a>Max Forbes

Max is a software engineer at Google in Seattle working on Kubernetes.

You can read more about his other projects and research at [maxwellforbes.com](http://maxwellforbes.com/).

<img src="http://dynamicinfradays.org/events/2015-boston/nick-gauthier.png" width="118" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="nickg"></a>Nick Gauthier

Nick Gauthier is a web developer who started with Rails, moved to the front end with JavaScript, then came back to the back end with Go.

He works at Codeship, a Continuous Delivery product company, on their new Docker-based platform.

<img src="http://dynamicinfradays.org/events/2015-boston/kir-kolyshkin.png" width="115" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="kirk"></a>Kir Kolyshkin

Kir was named leader and project manager for the OpenVZ project in 2005 to further the adoption of containers virtualization for Linux. He spearheads the overall development and manages all key architecture, updates and feature upgrades for OpenVZ.

Kir has more than 10 years Linux experience and has long been an active open source advocate.

<img src="http://dynamicinfradays.org/events/2015-boston/barak-michener.png" width="114" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="barakm"></a>Barak Michener

Barak is a distributed systems developer for CoreOS, working in Go on etcd.

His other interests include graph databases (maintaining Cayley), machine learning, and programming languages.

<img src="http://dynamicinfradays.org/events/2015-boston/igor-moochnick.png" width="115" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="igorm"></a>Igor Moochnick

Igor has been building enterprise cross-platform and cross-technology distributed systems for more than 20 years. He is passionate about all the technologies and methodologies that can enable applications to scale seamlessly, to process large amounts of data, and to serve more customers.

As a hands-on Cloud architect, Igor works with the teams to improve their development processes, increasing their effectiveness through the adoption of the Cloud-enabling technologies, Agile practices, DevOps processes and automation tool-chains.

In his spare time he blogs, geeks out on Big Data and Robotics, and is a frequent speaker and supporter for multiple code camps and events.

<img src="http://dynamicinfradays.org/events/2015-boston/jerome-petazzoni.png" width="113" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="jeromep"></a>J&eacute;r&ocirc;me Petazzoni

J&eacute;r&ocirc;me is a senior engineer at Docker, where he helps others to containerize all the things. In another life he built and operated Xen clouds when EC2 was just the name of a plane, developed a GIS to deploy fiber interconnects through the French subway, managed commando deployments of large-scale video streaming systems in bandwidth-constrained environments such as conference centers, operated and scaled the dotCloud PaaS, and various other feats of technical wizardry.

When annoyed, he threatens to replace things with a very small shell script.

<img src="http://dynamicinfradays.org/events/2015-boston/stephen-salinas.png" width="113" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="stephens"></a>Stephen Salinas

Stephen Salinas is an Infrastructure engineer at HubSpot in Cambridge, MA.

He's a contributor to Singularity, an open-source Mesos scheduling framework.

<img src="http://dynamicinfradays.org/events/2015-boston/joe-stein.png" width="113" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="joes"></a>Joe Stein

Joe Stein is the CEO of Elodina, Inc., a startup focusing on the support & maintenance of third party open source software, and also Founder and Principal Consultant of Big Data Open Source Security. Joe has been working for the last couple of years on implementing and assisting organizations with their Kafka, Mesos, Hadoop, Cassandra, Accumulo, Storm, Spark, etc. Big Data systems.

Prior to this, Joe Stein was responsible for building out a platform that ingested and processed the analytics for 6 billion unique mobile devices.

<img src="http://dynamicinfradays.org/events/2015-boston/jeff-victor.png" width="112" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="jeffv"></a>Jeff Victor

Jeff's 28-year computer career has included software development, system and network administration, and consulting. He was the Principal Author of the book _Solaris 10 System Virtualization Essentials_, and the creator of the Solaris Zones FAQ and the 'zonestat' open-source program.

Jeff received a Bachelor of Science degree (Computer Science) from Rensselaer Polytechnic Institute in Troy, New York. In his spare time, he builds and launches high-power rockets and manages automated wildlife cameras. He lives in New York with his wife and daughter.

His blog can be found at [blogs.oracle.com/jeffv](http://blogs.oracle.com/jeffv).

<img src="http://dynamicinfradays.org/events/2015-boston/tara-walker.png" width="114" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="taraw"></a>Tara Walker

Tara is a Technical Evangelist for Amazon Web Services, dedicating her time to help developers build apps in the AWS Cloud. Tara has most recently been working on evangelizing cross-platform development and AWS Mobile Services in conjunction with AWS Mobile team.

Tara has been spreading the "good news" about various development platforms and languages for over 15 years as a developer evangelist at Microsoft and various other Fortune 500 companies. During that time, she has had an opportunity to work with a myriad of technologies, languages, and frameworks for mobile, gaming, cloud, web, and NUI development.

You can find Tara on Twitter at [@taraw](https://twitter.com/taraw).

### Workshops

<img src="http://dynamicinfradays.org/events/2015-boston/boyd-hemphill.png" width="113" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="firstc"></a>_Deploy Your First Container to CoreOS, Cloud Foundry, Azure and AWS_ <span style="font-size: smaller">- 4h, Beginner</span>

Bring your laptop and get ready! We are going to help you give birth to your first baby container. First, you will learn about the Docker CLI, Dockerfile, and how to push your image to a Docker Registry.

Then you will learn how to deploy your container to multiple targets such as CoreOS, Cloud Foundry, Azure or AWS.

Led by Boyd Hemphill, StackEngine, [Barak Michener](#barakm), CoreOS and Dave Nielsen, CloudCamp

**Prerequisities**

Please ensure you have the following tools installed on your system:

* If you're running Mac OS X or Windows, [boot2docker](http://boot2docker.io/)

[more info](http://stackengine.com/docker-101-01-docker-development-environments/)

<img src="http://dynamicinfradays.org/events/2015-boston/jonas-rosland.png" width="112" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="dcpana"></a>_Creating Multi-container Apps with Docker Compose and Panamax_ <span style="font-size: smaller">- 2h, Intermediate</span>

So you've run a few standalone containers, now it's time to start piecing them together! Learn how to use Docker Compose and Panamax.io to create real multi-container apps.

Led by Jonas Rosland, EMCcode

**Prerequisities**

Please ensure you have the following tools installed on your system:

* If you're running Mac OS X or Windows, [boot2docker](http://boot2docker.io/)
* [Docker Compose](https://docs.docker.com/compose/install/#install-compose)
* [Panamax](http://panamax.io/get-panamax/)

[slides](http://www.slideshare.net/jonasrosland/docker-compose-and-panamax-containerdays-boston-june-2015)

<img src="http://dynamicinfradays.org/events/2015-boston/borja-burgos.png" width="113" height="140" style="margin-left:10px; margin-bottom: 5px; float:right; clear: right;">

#### <a name="tutum"></a>_Continuous Delivery & Management of your Multi-container Apps with DockerHub and Tutum_ <span style="font-size: smaller">- 2h, Intermediate</span>

Learn how to use DockerHub and Tutum to automate the delivery of your multi-container applications across any infrastructure.

Led by Borja Burgos, Tutum

**Prerequisities**

Please ensure you have the following tools installed on your system:

* If you're running Mac OS X or Windows, [boot2docker](http://boot2docker.io/)
* [Docker Compose](https://docs.docker.com/compose/install/#install-compose)

[slides](http://www.slideshare.net/borjaburgos/containerdays-2015) [more info](http://blog.tutum.co/2015/06/08/blue-green-deployment-using-containers/)

<img src="http://dynamicinfradays.org/img/logo.png" height="120" width="232" style="margin: 40px auto 20px auto; display: block;">

<div style="text-align: center; display: block;"><em><strong>ContainerDays Boston 2015</strong> is a <a href="http://dynamicinfradays.org">DynamicInfraDays</a> event</em></div>
