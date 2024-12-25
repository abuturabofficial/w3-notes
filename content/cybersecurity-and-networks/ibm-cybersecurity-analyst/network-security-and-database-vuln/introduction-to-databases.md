---
title: "Introduction to Databases"
date: 2023-03-21 12:23:00 +0500
LastModifierDisplayName: AbuTurab
LastModifierEmail: cyberfrontofficial@proton.me
collapsibleMenu: true
alwaysOpen: false
weight: 3
---

## **Data Source Types**

- Distributed Databases
	- Microsoft SQL Server, DB2, Oracle, MySQL, SQLite, Postgres etc.
	- Structured Data
- Data Warehouses
	- Amazon’s redshift, Netezza, Exadata, Apache Hive etc.
	- Structured Data
- Big Data
	- Google BigTable, Hadoop, MongoDB etc.
	- Semi-Structured Data
- File Shares
	- NAS (Network Attached Storage), Network fileshares such as EMC or NetApp; and Cloud Shares such as Amazon S3, Google Drive, Dropbox, Box.com etc.
	- Unstructured-Data
	  
	  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases.png)

## **Data Model Types**

### Structured Data
  
  “Structured data is data that has been organized into a formatted repository, typically a database, so that its elements can be made addressable for more effective processing and analysis.”

### Semi-Structured Data
  
  “Semi-structured data is data that has not been organized into a specialized repository, such as a database, but that nevertheless has associated information, such as metadata, that makes it more amenable to processing than raw data.”
- A Word document with tags and keywords.

### **Unstructured Data**
  
  “Unstructured data is information, in many forms, that doesn’t hew to conventional data models and thus typically isn’t a good fit for a mainstream relational database.”
- A Word Document, transaction data etc.

#### Types of Unstructured Data

- Text (most common type)
- Images
- Audio
- Video

## **Structured Data**

### Flat File Databases
  
  Flat-file databases take all the information from all the records and store everything in one table.
- This works fine when you have some records related to a single topic, such as a person’s name and phone numbers.
- But if you have hundreds or thousands of records, each with a number of fields, the database quickly becomes difficult to use.

### Relational Databases
  
  Relational databases separate a mass of information into numerous **tables**. All columns in each table should be about one topic, such as “student information”, “class Information”, or “trainer information”.
- The tables for a relational database are linked to each other through the use of **Keys**. Each table may have one **primary key** and any number of **foreign keys**. A **foreign key** is simply a **primary key** from one table that has been placed in another table.
- The most important rules for designing relational databases are called **Normal Forms**. When databases are designed properly, huge amounts of information can be kept under control. This lets you **query** the database (search for information section) and quickly get the answer you need.
  
  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases-1.png)

# **Securing Databases**

## **Securing your “Crown Jewels”**
  
  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases-2.png)

## Leveraging Security Industry Best Practices
  
  **Enforce:**
- DOD STIG
- CIS (Center for Internet Security)
- CVE (Common Vulnerability and Exposures)
  
  **Secure:**
- Privileges
- Configuration settings
- Security patches
- Password policies
- OS level file permission
  
  **Established Baseline:**
  User defined queries for custom tests to meet baseline for;
- Organization
- Industry
- Application
- Ownership and access for your files
  
  **Forensics:**
  Advanced Forensics and Analytics using custom reports
- Understand your sensitive data risk and exposure

## **Structured Data and Relational Databases**
  
  Perhaps the most common day-to-day use case for a database is using it as the backend of an application, such as your organization HR system, or even your organization's email system!
  
  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases-3.png)

## **Anatomy of a Vulnerability Assessment Test Report**
  
  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases-4.png)

## **Securing Data Sources by Type**
  
  ![Introduction to Databases](/notes/ibm-cybersecurity-analyst/Introduction%20to%20Databases-5.png)

# **A Data Protection Solution Example, IBM Security Guadium Use Cases**

## **Data Monitoring**

### Data Activity Monitoring/Auditing/Logging

- Does your product log all key activity generation, retrieval/usage, etc.?
- Demo data access activity monitoring and logging of the activity monitoring?
- Does your product monitor for unique user identities (including highly privileged users such as admins and developers) with access to the data?
- At the storage level, can it detect/identify access to highly privileged users such as database admins, system admins or developers?
- Does your product generate real time alerts of policy violations while recording activities?
- Does your product monitor user data access activity in real time with customizable security alerts and blocking unacceptable user behavior, access patterns or geographic access, etc.? If yes, please describe.
- Does your product generate alerts?
- Demo the capability for reporting and metrics using information logged.
- Does your product create auditable reports of data access and security events with customizable details that can address defined regulations or standard audit process requirements? If yes, please describe.
- Does your product support the ability to log security events to a centralized security incident and event management (SIEM) system?
- Demo monitoring of non-Relational Database Management Systems (nRDBMS) systems, such as Cognos, Hadoop, Spark, etc.
