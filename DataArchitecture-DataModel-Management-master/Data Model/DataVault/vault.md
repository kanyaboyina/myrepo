# Data Vault Organization of Objects:

* **HUB**        -  Consists of unique list of Business Keys and Multi Tenancy 
* **SATELLITE**  - Consists of descriptive data of parent Hub or Link that can change over time
* **LINK**       - Represents relationships/associations, hierarchies, transactions and events

![image](https://github.tfs.toyota.com/storage/user/793/files/756f535e-de35-11ea-8256-bfb65ce01b16) ![image](https://github.tfs.toyota.com/storage/user/793/files/9185cbc2-de35-11ea-9b4c-a6c29d23f277) 
![image](https://github.tfs.toyota.com/storage/user/793/files/c47a1060-de35-11ea-8230-3a4ba5c05995)
-----

# Data Vault – Overview of Data Model
![image](https://github.tfs.toyota.com/storage/user/793/files/40a9ba0e-e210-11ea-935a-978af21dab97)
------

# Data Vault – Multi Tenancy and Product Line of Business

 ### **Multi Tenancy:**

* Data segregation at Hub level with Tenant ID

* Different Vaults

* Different S3 buckets

### **Product Line of Business:**

* Data segregation by Domain 
 Example: Insurance, Commercial Finance, Consumer Finance, etc.

* Introducing Hubs, Satellites and Links by Product Line of Business ![image](https://github.tfs.toyota.com/storage/user/793/files/0efa5cb0-e211-11ea-890c-0201370505d2)
------

# Data Vault – POC Data Model based on CCP

![image](https://github.tfs.toyota.com/storage/user/793/files/1d7cd9d6-e214-11ea-84a4-f81646e36ec7)
-----------

# Data Vault – Example of Hub & Satellite

![image](https://github.tfs.toyota.com/storage/user/793/files/cf0faeae-e213-11ea-8be7-3ab7e6792fd3)
------------

# Data Vault – Example of Link & Link Satellite

![image](https://github.tfs.toyota.com/storage/user/793/files/6d7e56a8-e214-11ea-899d-71443893a2de)
-------

# Data Vault – Loading Strategy

![image](https://github.tfs.toyota.com/storage/user/793/files/87e371d6-e214-11ea-8553-6853189dba55)
------







