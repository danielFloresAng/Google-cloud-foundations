// Google cloud data storage

<!--
  Every application needs to store data,and different applications and workloads require different storage database solutions.
  Google Cloud offers relational and non-relational databases and worldwide object storage.
 -->

Google Cloud provides managed storage and database that include:

- Cloud Storage
- Cloud SQL
- Cloud Spanner
- Firestore
- Cloud Bigtable

<!-- Unstructured and structured Data -->

<Unstructured-data is information stored in a non-tabular form such as documents, images, and audio files. Is usually best suited to Cloud Storage.>

<Structured-data represents information stored in tables, rows, and columns. We can expect this type of data to be organized and clearly defined and usually easy to capture, access, and analyze.>
Structured data comes in two types: transactional workloads and analytical workloads.

- - - > Transactional workloads stem from Online Transaction Processing systems, which are used when fast data inserts and updates are required to build row-based records.

- - - > Analytical workloads, which stem from Online Analytical Processing systems, which are used when entire datasets need to be read.

<Cloud-Storage is a fully managed scalable service that has a wide variety of uses. A few examples include serving website content, storing data for archival and disaster recovery, and distributing large data objects to end users through Direct Download.>

There are four primary storage classes in Cloud Storage, and stored data is managed and billed according to which class it belongs in:

- Standard Storage: is considered best for frequently accessed, or “hot,” data.
  It’s also great for data that is stored for only brief periods of time.

- Nearline Storage: this is best for storing infrequently accessed data, like reading or modifying data once per month on average.
  Examples include data backups, long-tail multimedia content, or data archiving.

- Coldline Storage: this is also a low-cost option for storing infrequently accessed data. However, as compared to Nearline Storage, Coldline Storage is meant for reading or modifying data, at most, once every 90 days.

- Archive Storage: this is the lowest-cost option, used ideally for data archiving, online backup, and disaster recovery.It’s the best choice for data that you plan to access less than once a year,because it has higher costs for data access and operations and a 365-day minimum storage duration.

<!-- Cloud Storage files are organized into buckets.
A bucket needs a globally unique name and a specific geographic location for where it should be stored, and an ideal location for a bucket is where latency is minimized.
-->

<!-- SQL Managed services -->

<Cloud-SQL offers fully managed relational databases, including MySQL, PostgreSQL, and SQL Server as a service. It’s designed to hand off mundane, but necessary and often time-consuming, tasks to Google—like applying>

<Cloud-Spanner is a fully managed relational database service that scales horizontally, is strongly consistent, and speaks SQL. Vertical scaling is where you make a single instance larger or smaller, while horizontal scaling is when you scale by adding and removing servers. Cloud Spanner users are often in the advertising, finance, and marketing technology industries, where they need to manage end-user metadata.>

<!-- NoSQL Managed services -->

<Firestore is a flexible, horizontally scalable, NoSQL cloud database for mobile, web, and server development. With Firestore, incoming data is stored in a document structure, and these documents are then organized into collections. Documents can contain complex nested objects in addition to subcollections.>

<Bigtable is Google is NoSQL big data database service. It is the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail.Bigtable is designed to handle massive workloads at consistent low latency and high throughput, so it is a great choice for both operational and analytical applications, including Internet of Things, user analytics, and financial data analysis.>

/// API (Application programing interface)

<!--
  A software is structured so that it presents a clean, well-defined interface that hides unnecessary detail, and then they document that interface.
  That's an API.
 -->

> REST (REpresentational State Transfer): is currently the most popular architectural style for services.

/// Cloud endpoints.

Cloud Endpoints is a distributed API management system that uses a distributed Extensible Service Proxy, which is a service proxy that runs in its own Docker container.

/// Apigee API
Unlike Cloud Endpoints, Apigee API Management has a specific focus on business problems, like rate limiting, quotas, and analytics.
In fact, many Apigee API Management users provide a software service to other companies.

<Pub/Sub, a Google Cloud asynchronous messaging service and API that supports distributed message-oriented architectures at scale. One of the early stages in a data pipeline is data ingestion, which is where large amounts of streaming data are received. PubSub is a distributed messaging service that can receive messages from various device streams such as gaming events, IoT devices, and application streams. PubSub ensures at-least-once delivery of received messages to subscribing applications, with no provisioning required. PubSub’s APIs are open, the service is global by default, and it offers end-to-end encryption.>

- A central element of Pub/Sub is the topic.
  <!--
    A topic is a named resource to which messages are sent by publishers. You can think of a topic like a radio antenna. Whether your radio is playing music or it’s turned off, the antenna itself is always there. If music is being broadcast on a frequency that nobody’s listening to, the stream of music still exists.
    Similarly, a publisher can send data to a topic that has no subscriber to receive it.
    -->

<!-- YOU CAN'T SECURE THE CLOUD, RIGHT? -->

Google provides fiver layers of protection to keep customers' data safe:

- Hardware infrastructure
- Service deployment
- Storage services
- Internet communication
- Operational security

Google cloud offers 3 options to encrypt data:

- Google Cloud default encryption

- Customer-managed encryption keys (CMEK)
  <Cloud Key Management Service, or Cloud KMS, automates and simplifies the generation and management of encryption keys. The keys are managed by the customer and never leave the cloud. Cloud KMS supports encryption, decryption, signing, and verification of data.>

- Customer-supplied encryption keys (CSEK).
  <Customer-supplied encryption keys give users more control over their keys, but with greater management complexity. With CSEK, users use their own AES 256-bit encryption keys. They are responsible for generating these keys. Users are responsible for storing the keys and providing them as part of Google Cloud API calls. Google Cloud will use the provided key to encrypt the data before saving it. Google guarantees that the key only exists in-memory and is discarded after use.>

- IAM (Identity and Access Management):
  <With IAM, administrators can apply policies that define who can do what on which resources. The “who” part of an IAM policy can be a Google Account, a Google group, a service account, or Cloud Identity domain. The “can do what” part of an IAM policy is defined by a role. An IAM role is a collection of permissions.>

  There are three kinds of roles in IAM:

  - Basic:
    Project viewers can examine resources, but can’t modify them. Project editors can examine and modify a resource. And project owners can also examine and modify a resource. In addition, project owners can manage the associate roles and permissions, and set up billing.

  - Predefined:
    Provides other ways to assign permissions that are more specifically tailored to meet the needs of typical job roles.

  - Custom.
    It allow to create custom roles that have specifict permissions

    <Identity-Aware Proxy, or IAP, is a resource that can be used to set up authentication to https-based applications without the use of VPNs.>
