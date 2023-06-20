---
title: ""
date: 2023-06-16T22:00:08-06:00
description: "Principal DevOps Engineer, NICE CXone"
draft: false
featured_image: '/images/llama.jpg'
---

Education
---------

May 2015:   **B.S., Computer Science**; Weber State University (Ogden, Utah)

Experience
----------

**NICE CXone: Principal DevOps Engineer**
09/2020 - Present

I am the lead engineer on my team of 14 engineers and I have unofficially worn the manager hat for the last 2 years
while we have not had a manager. We recently got a manager! My team is responsible for building and sustaining
solutions which make our internal developer’s lives easier. Our main responsibilities include:

* Maintain an EKS platform shared by many developers for hosting their workloads
* Create reusable Helm charts to simplify how workloads are deployed in our EKS platform
* Manage AWS IAM access for both humans and services
* Create reusable GitHub Actions workflows to simplify common CI tasks
* Maintain a shared Jenkins infrastructure
* Automate the deployment of IAC for various developer teams

Maintaining and improving our AWS EKS platform accounts for a large portion of the work done by my team. This
internal platform as a service is shared for the hosting of all workloads created by our R&D department. My
team maintains the clusters, many shared components within the clusters (Karpenter, Prometheus, AWS Load
Balancer Controller, etc), and CD process and tooling for deploying workloads. The project to provision
this infrastructure started in December 2020. All of the infrastructure (VPC, EKS, Node Groups, ALBs, S3,
Route53, WAF) is provisioned using Terraform within GitHub Actions workflows. All the workloads are provisioned
using Helm charts or Kustomize overlays synced by ArgoCD. We follow a strict GitOps approach for deploying all
workloads. I was the only engineer assigned to build this infrastructure when the project started. There are now
14 engineers supporting this project. Before this infrastructure, R&D engineers were required to create their own
hosting infrastructure unique per each workload. I have been influential in helping the R&D organization to
standardize on a common way of deploying workloads. This has been hugely beneficial for reducing the effort to
get new microservices deployed and for standardizing our operational behavior and tooling.

**NICE CXone: Senior Software Engineer**
03/2019 - 09/2020

I worked on the development of various Go microservices designed to increase scalability of monolithic
applications through thoughtfully breaking out features. The services which we built are stateless and
integrate with AWS DynamoDB, SQS, and Kinesis for state management. I was an influential member of the
team in making technology decisions and standards for future development such as Kubernetes, Go, gRPC,
Stateless design pattern. I was the primary developer of our reusable CI/CD workflows which saved countless
hours of developer time. I was the primary developer of our Kubernetes platform, hosted on AWS EKS.

**NICE CXone: Senior Software Engineer**
09/2018 - 03/2019

I worked on the development of a Nice InContact core microservice written in Scala with Akka. While on this
team it was identified that there was a large gap in the monitoring of the health of this core microservice.
This microservice was deployed in a way that differed greatly from other solutions in the past. Due to these
differences our typical monitoring tools would not suffice. I wrote a small service which sends simulated
events through the microservice on a recurring interval to provide metrics on how the simulated events are
being processed. This monitoring service still serves today as the primary method of health visibility for
the Scala microservice and has served as a pattern of best practice for other developers writing microservices.

**NICE CXone: Senior Software Engineer**
12/2015 - 09/2018

I created and maintained applications (primarily in C# and Go) that are responsible for monitoring the stability
of the Nice inContact platform. If an internal service required monitoring that was not possible with one of our
existing solutions then I would build a custom solution. I also managed and configured our BMC TrueSight, Prometheus,
and Grafana monitoring tools. I developed methods of delivering production telemetry that are still heavily depended
on. I gained a strong knowledge of what it takes to operate production services and how to effectively produce
automated actions or alerts based upon problematic application behaviors.


**AdvancedMD: Software Engineer**
06/2015 - 12/2015

I worked on a team whose primary responsibility was to build integrations and new features on the NetSuite platform.
We used primarily vanilla javascript for most of our projects.

**Calldrip: Full Stack Web Developer**
02/2014 - 06/2015

Full stack developer. Designed, maintained, and created all web pages (PHP, HTML, CSS/Twitter Bootstrap,
Javascript/jQuery) and the database (mySQL) hosted on Google Cloud Computing. When I joined this company
their website was hosted on servers in a private data center and deployed by manually copying files into
the servers. I was influential in driving a migration to GCP infrastructure with our software deployed
via a custom automated process triggered by Git commits.

Technical Experience
--------------------

Copy To Read - Text to Speech
:   This is an Android app which I developed as a fun side project. The basic functionality of the app is to convert
copied text into audible speech (text to speech). This app has 100,000+ downloads spread across many countries.
I've enjoyed countless interactions with users of the app over the years.

Programming Languages
:   **Go:** I started working professionally with Go in 2017. I enjoy the simplistic syntax and simple SDLC that Go
supports. When starting a new project this is my go-to language. My most recent Go project was to create a GitHub App
hosted in Kubernetes which assigns and enforces code reviewers to GitHub Pull Requests. This project has greatly reduced
undesired GitHub notifications to users and the time it takes to get a Pull Request reviewed and merged.

:   **terraform:** I've been working professionally with terraform for about 5 years to provision primarily AWS resources.
I've worked with various terraform providers and modules over the years and constructed many of my own modules. My current
team provisions all of our AWS resources using a GitOps workflow built around Terraform.

:   **C#:** I started working professionally with C# in 2015. I have developed many applications used for monitoring the
health of other applications via Windows Performance Counters, HTTP APIs, SOAP APIs, gRPC APIs, and various other methods
which aren't supported by our vendor supplied monitoring tools.

:   **Java:** I started working with Java during College in 2013. My primary experience with Java has been to create my
Copy To Read Android app. Throughout my time at NICE CXone I've made some contributions to various Java projects.

:   Basic knowledge of **Python**, **YAML (Kubernetes!)**, **Helm**, **Groovy**, **Javascript**, **Typescript**, **Spanish**

