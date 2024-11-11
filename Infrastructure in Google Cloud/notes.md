// Google cloud data storage
<!--  
  Every application needs to store data,and different applications and workloads require different storage database solutions.
  Google Cloud offers relational and non-relational databases and worldwide object storage.
 -->

Google Cloud provides managed storage and database that include: 
  * Cloud Storage 
  * Cloud SQL 
  * Cloud Spanner 
  * Firestore
  * Cloud Bigtable
 
<!-- Unstructured and structured Data -->
  <Unstructured-data is information stored in a non-tabular form such as documents, images, and audio files. Is usually best suited to Cloud Storage.>

  <Structured-data represents information stored in tables, rows, and columns. We can expect this type of data to be organized and clearly defined and usually easy to capture, access, and analyze.>
    Structured data comes in two types: transactional workloads and analytical workloads.

- - - > Transactional workloads stem from Online Transaction Processing systems,  which are used when fast data inserts and updates are required to build row-based records.

- - - > Analytical workloads, which stem from Online Analytical Processing systems, which are used when entire datasets need to be read.


<Cloud-Storage is a fully managed scalable service that has a wide variety of uses. A few examples include serving website content, storing data for archival and disaster recovery, and distributing large data objects to end users through Direct Download.>

There are four primary storage classes in Cloud Storage, and stored data is managed and billed according to which class it belongs in:

  * Standard Storage: is considered best for frequently accessed, or “hot,” data.
  It’s also great for data that is stored for only brief periods of time.

  * Nearline Storage: this is best for storing infrequently accessed data,        like reading or modifying data once per month on average. 
  Examples include data backups, long-tail multimedia content, or data archiving.

  * Coldline Storage: this is also a low-cost option for storing infrequently accessed data. However, as compared to Nearline Storage, Coldline Storage is meant for reading or modifying data, at most, once every 90 days.

  * Archive Storage: this is the lowest-cost option, used ideally for data archiving, online backup, and disaster recovery.It’s the best choice for data that you plan to access less than once a year,because it has higher costs for data access and operations and a 365-day minimum storage duration.

<!-- Cloud Storage files are organized into buckets.
A bucket needs a globally unique name and a specific geographic location for where it should be stored, and an ideal location for a bucket is where latency is minimized. 
-->

<!-- SQL Managed services -->

  <Cloud-SQL offers fully managed relational databases, including MySQL, PostgreSQL, and SQL Server as a service. It’s designed to hand off mundane, but necessary and often time-consuming, tasks to Google—like applying>

  <Cloud-Spanner is a fully managed relational database service that scales horizontally, is strongly consistent, and speaks SQL. Vertical scaling is where you make a single instance larger or smaller, while horizontal scaling is when you scale by adding and removing servers. Cloud Spanner users are often in the advertising, finance, and marketing technology industries, where they need to manage end-user metadata.>

<!-- NoSQL Managed services -->  

  <Firestore is a flexible, horizontally scalable, NoSQL cloud database for mobile, web, and server development. With Firestore, incoming data is stored in a document structure, and these documents are then organized into collections.  Documents can contain complex nested objects in addition to subcollections.>

  <Bigtable is Google is NoSQL big data database service. It is the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail.Bigtable is designed to handle massive workloads at consistent low latency and high throughput, so it is a great choice for both operational and analytical applications, including Internet of Things, user analytics, and financial data analysis.>