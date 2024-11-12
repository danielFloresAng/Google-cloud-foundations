<!-- what's the cloud? -->

Cloud computing is a way of using IT that has these five equally important traits"
1.- Customers get computing resources that are on-demand and self-service
2.- Get access to those resources over the internet, from anywhere
3.- The provider of those resources allocates them to users out of that pool
4.- The resources are elastic-which means they can increase or decrease as needed
5.- Customers pay only for what they use, or reserve as they go

Components:

- Users
- Applications
- Infrastructure

// IaaS, PaaS and SaaS

- IaaS: Infrastructure as a service
- PaaS: Platform as a service
- ISaaS: Software as a service

// Google cloud Infrastructure are based on three layers

1- Networking and security
2- Compute and storage
3- Big data and ML products

- Google cloud computing Services:

  - Compute engine
  - Google kubernets engine
  - App engine
  - Cloud functions
  - Cloud run

- Google cloud storage services:
  - Cloud storage
  - Cloud SQL
  - Cloud spanner
  - Cloud Bigtable
  - Firestore

<!-- MODULE 2 -->

There are four ways to interact with google cloud:

- Google cloud console
- Cloud SDK and cloud shell
- APIs
- Cloud mobile app

The Google Cloud console, which is Google Cloud’s Graphical User Interface (GUI), helps you deploy, scale, and diagnose production issues in a simple web-based interface.
To access the console, navigate to <console.cloud.google.com.>

The console is used to access and use resources, and those resources are organized in projects.
The Google Cloud resource hierarchy is made up of four levels:

- resources
- projects
- folders
- organization node

  //Projects attributes vary in uniqueness and immutability

  A Google Cloud project is an organizing entity for your Google Cloud resources. It often contains resources and services; for example, it may hold a pool of virtual machines, a set of databases, and a network that connects them together. Projects also contain settings and permissions, which specify security rules and who has access to what resources.

  - Project ID (immutable)
  - project name (mutable)
  - Project number (immutable)

// Google coud billing

Wwhen you define a Google Cloud project, you link a billing account to it.
This billing account is where you will configure all your billing information, including your payment option.

There are two types of quotas:

- Rate quotas: reset after a specific time.
- Allocation quotas: govern the number of resources you can have in your projects.

// Cloud software development kit (SDK)
<SDK lets users run Google Cloud command-line tools from a local desktop. >

The SDK tools includes:

- the gcloud CLI, which provides the main command-line interface for Google Cloud products and services.
- gsutil (g-s-util), which lets you access Cloud Storage from the command line.
- bq, a command-line tool for BigQuery.

<Cloud Shell provides command-line access to cloud resources directly from a browser.>

<App Engine lets you build highly scalable applications on a fully managed, serverless platform.>
With App Engine, you can choose from popular coding languages, libraries, and frameworks to develop apps

// Cloud functions
Is serverless code that let you run it based on certain events

//Google kubernetes engine (GKE)
provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The GKE environment consists of multiple machines (specifically Compute Engine instances) grouped to form a container cluster.

//Gloud Run
Manage compute platform that less run stateless containers by using web request or Pub sub events. Is serverless

Google cloud run workflow is a three-steps process:

- Write the application code
- Build and packege the application into a container image
- Deploy the container image to cloud run
