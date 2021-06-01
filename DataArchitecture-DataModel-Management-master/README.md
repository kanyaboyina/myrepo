# DataArchitecture-DataModel-Management
Enterprise Data management for Platform Enablement

## Goal :

Office of the  Data Architecture and Data Modelling practice is to enable the  building of a world class system and industry leading data platform

## Purpose :

* Design data structures to meet integration demands
* Standardize Data and Information architecture to align with Data Standards
* Enforce Data Quality, Data Security & Data Storage standards
* Manage and govern TFS Data Model • Enforce TFS Reference & Master Data rules
* Validate Data Model against Functional and Process needs
* Interact regularly with Enterprise Architecture, Internal and External partners
* Raise issues for items that don’t follow guidelines and standards

Table of Contents
=================

* [Essential components](#Essential-components)
  * [Data Modeling and Data Architecture](#Data-Modeling-and-Data-Architecture)
* [Data Models](#Data-Model)
  * [Data Vault](#Data-Vault) 
* [DataArchitecture](#Data-Architecture)
* [Enterprise Data Platform (EDP)](#Enterprise-Data-Platform-(EDP))
  * [EDP 2.0](#EDP-2.0)



--------


# Essential components <a name="Essential-components"></a>


# Data Modeling and Data Architecture <a name="Data-Modeling-and-Data-Architecture"></a>
Information modeling describes the metadata necessary to understand the data, processes and rules that are relevant to the enterprise (Figure 1). Information modeling has three main domains: 

**Data Modeling** : the logical data model is the definition of business terms and context of usage of a data element. For example, party data that can group customer and prospect entities.

**Process Modeling** : the definition of the enterprise business processes that the enterprise uses. Process modeling uses data model entities and describes how data is created, or transformed, through the business process. For example, the process through which a prospect becomes a customer.

**Rule Modeling** : describes the data governance and compliance policies for the entire organization. Rules describe the quality and regulatory rules that data must follow to be aligned with corporate policies. For example, a customer must be older than 21, or any data item that is over five years old needs to be archived. 


**Data Architecture** :  defines the data along with the schemas, integration, transformations, storage, and workflow required to enable the  requirements of the information architecture. A solid data architecture is a blueprint that helps align your company’s data with its business strategies. The data architecture guides how the data is collected, integrated, enhanced, stored, and delivered to business stakeholder who use it to do their jobs. It helps make data available, accurate, and complete so it can be used for business decision-making.


![image](https://github.tfs.toyota.com/storage/user/793/files/7689e7b0-e7bb-11ea-87f7-0f380c72bba7)


ref: https://sites.google.com/site/aniketsaoblog/home/data-information-architecture-layer/information-architecture-essential-components




# Enterprise Data Platform (EDP) <a name="Enterprise-Data-Platform-(EDP)"></a>

## EDP 2.0 <a name="EDP-2.0"></a>

**Conceptual View : First Level**

![image](https://github.tfs.toyota.com/storage/user/793/files/17a5a344-ec4b-11ea-9ccf-42ac4403bcf5)


**Conceptual View : Second Level**

![image](https://github.tfs.toyota.com/storage/user/793/files/4739bab4-ec4b-11ea-8a95-b36d3564a033)








# Data Model <a name="Data-Model"></a>

## Data Vault  <a name="Data-Vault"></a>


### Data Vault Organization of Objects:

* **HUB**        -  Consists of unique list of Business Keys and Multi Tenancy 
* **SATELLITE**  - Consists of descriptive data of parent Hub or Link that can change over time
* **LINK**       - Represents relationships/associations, hierarchies, transactions and events

![image](https://github.tfs.toyota.com/storage/user/793/files/756f535e-de35-11ea-8256-bfb65ce01b16) ![image](https://github.tfs.toyota.com/storage/user/793/files/9185cbc2-de35-11ea-9b4c-a6c29d23f277) 
![image](https://github.tfs.toyota.com/storage/user/793/files/c47a1060-de35-11ea-8230-3a4ba5c05995)
-----

## Data Vault – Overview of Data Model
![image](https://github.tfs.toyota.com/storage/user/793/files/40a9ba0e-e210-11ea-935a-978af21dab97)
------

## Data Vault – Multi Tenancy and Product Line of Business

 ### **Multi Tenancy:**

* Data segregation at Hub level with Tenant ID

* Different Vaults

* Different S3 buckets

### **Product Line of Business:**

* Data segregation by Domain 
 Example: Insurance, Commercial Finance, Consumer Finance, etc.

* Introducing Hubs, Satellites and Links by Product Line of Business ![image](https://github.tfs.toyota.com/storage/user/793/files/0efa5cb0-e211-11ea-890c-0201370505d2)
------

## Data Vault – POC Data Model based on CCP

![image](https://github.tfs.toyota.com/storage/user/793/files/1d7cd9d6-e214-11ea-84a4-f81646e36ec7)
-----------

## Data Vault – Example of Hub & Satellite

![image](https://github.tfs.toyota.com/storage/user/793/files/cf0faeae-e213-11ea-8be7-3ab7e6792fd3)
------------

## Data Vault – Example of Link & Link Satellite

![image](https://github.tfs.toyota.com/storage/user/793/files/6d7e56a8-e214-11ea-899d-71443893a2de)
-------

## Data Vault – Loading Strategy

![image](https://github.tfs.toyota.com/storage/user/793/files/87e371d6-e214-11ea-8553-6853189dba55)
------

