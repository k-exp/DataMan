# DataMan
Decentralized peer-to-peer dataset management package using IFPS and ethereum smart contracts. 

## Overview and Philosophy
If we are working on a project with multiple people that require a shared dataset, there are multiple solutions. The classic solution is to have a hosted database to which all parties can connect to. In an effort to always stay lean, a more appealing approach is to utilize the resources we have readily available, our personal computers, to share the data in a peer-to-peer network so we can cut out this hosted centralized resource which is often costly to maintain. 

DataMan is a data management system that strives for simplicity and robustness. We use IFPS as the distributed architecture for sharing files and use ethereum to grant access. 

## Problems to Solve
* Securely sharing data.
* Reducing need for centralized hosted data storage solution. 
* Improving peer-to-peer resource utilization. 

## Solutions
Several platforms exist to solve the problems stated above; however, they do not solve it in the way we wish to solve it. Generally all these methods have some centralized authority and host.

### Keybase File System (KBFS)
Our team has been using the keybase filesystem to securely share datasets for about a month now. Data is encrypted and stored on a keybase server. This requires keybase to share an immense hosting responsibility. As of now, there is no fees or perceivable limits, but that does not seem economical in the long term. 
* https://keybase.io/docs/kbfs

### Google Drive, One Drive, Drop Box etc.
There are many data hosting services with friendly interfaces. If budget is no issue,this is a solid method, as your data has some expectation of security by the provider. 
* https://www.dropbox.com/
* https://www.google.com/drive/

### Blob Storage / S3 and Metadata Store
S3 is a very economical way to host and share large datasets. Generally, you use one database like MongoDB to store dataset metadata and S3 to store the associated blob files (ie. images). 
* https://aws.amazon.com/s3/
* https://www.mongodb.com/

### Encrypted Torrents
DataMan is mainly meant to expand upon the properties and capabilities of encrypted torrents. One clear main advantage of the marriage of IFPS and ethereum is transactional security and accountability. These ideas will be developed more here. 
