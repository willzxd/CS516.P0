# Project 0
Xiaodan Zhu
<br />Date: Jan 25, 2015
<br />Version: 1.0
<br />

Project requirement:<br />
For every single system listed in the “DataPlatformsMap”, give as a list of succinct points:*  Strengths (with numbered references)*  Weaknesses (with numbered references)*  References (can be articles, blog posts, research papers, white papers, your own assessment, ...)
- - -
- - - 
## Introduction
I try to trace different routines mentioned on this map. And I am more interested in what I have never heard.

- - -
- - -

## Analysis of dataplatforms
- - -

### Database.com
* Relational
* SaaS,PaaS
* MySQL ecosystem

#### Strengths
* "The world's most trusted and secure cloud database", said by itself.
* It is a esay-use cloud database engine for mobile and social applications [1][1].
* It return JSON format for queries [1][1].
* The platform supports many different programm languages, such as Java, C, C#, Ruby, Python, PHP, etc.
* It has a quickstart instruction and an example written by Java, which helps developer begin to work on it quickly [2][2].
* It has a user-friendly user interface [2][2].
* Cheap

[1]: https://bighadoop.wordpress.com/2013/10/14/database-com-salesforce-coms-cloud-database/
[2]: http://www.salesforce.com/us/developer/docs/workbook_database/
#### Weaknesses
* It is not perform well, if some company want to build a data-intensive system by using Database.com. Internet latency is a big problem.[3][3]
* I doubt the security of this platform becasue it only combine lots of regular policy together. There are no advanced technology to prove that it is "the world's most trusted and secure cloud database" [4][4].
* The website terribly works in Safari [5][5]. If a company cannot properly show the contents of website, it is difficult for me to trust its products.

[3]: http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html
[4]:https://trust.salesforce.com/trust/practices/
[5]: http://www.salesforce.com/platform/services/

- - -
### Azure SQL Database
* A relational database-as-a-service [7][7]<br />
* Renamed version of SQL Azure [6][6]

#### Strengths
* Part of Microsoft Azure [7][7]
* Using a special version of Microsoft SQL Sever as its backend [8][8]
* Making relational queries which is structured or semi-structured, or even unstructured documents [8][8]
* Scalable service plans for multiple needs and budgets [9][9]. 
* Support popular tools for SQL developers [9][9]
* Support for VM [9][9]
* Fundemental price is resonable. [9][9]
* Support for non-Microsoft technologies [9][9]
* Migrating from SQL Server easily [9][9]

[6]: http://searchsqlserver.techtarget.com/essentialguide/Evolution-of-Windows-Azure-SQL-Database
[7]: http://azure.microsoft.com/en-us/services/sql-database/
[8]: http://en.wikipedia.org/wiki/SQL_Azure
[9]: http://searchsqlserver.techtarget.com/feature/The-pros-of-Windows-Azure-SQL-Database
#### Weaknesses
* Lots of T-SQL features do not be implemented [10][10]
* Extra charge [10][10]
* Security Probems [11][11] (For example, it does not support encrypting transparent data [10][10].) 

[10]: http://searchsqlserver.techtarget.com/feature/Why-you-should-think-twice-about-Windows-Azure-SQL-Database
[11]: http://searchsqlserver.techtarget.com/feature/SQL-Azure-security-terrifies-IT-but-loss-of-control-might-be-real-fear 
- - -
### ClearDB
* DaaS
* Part of MySQL ecosystem

#### Strengths
* Geo distributed cloud database system[12][12]
* Safety (Backup globally)[12][12]
* That Database is next to applications eliminates latency issuses.[12][12]

[12]:https://www.cleardb.com/better.view
#### Weakneeses
* Features is not many as some other DaaS.[13][13]

[13]:http://stackshare.io/stackups/amazon-rds-vs-cleardb-vs-google-cloud-sql
---
###ASW RDU
Part of MySQL ecosystem

#### Strengths
* The most interesting point is which is better comparing with EC2 for MySQL. Based on some articles, generally the peroformance of RDU is a bit better than EC2 for MySQL [14][14] [15][15].
* Growing support for different database systems, such as PostgreSQL, Oracle Database, SQL Server. [16][16]

#### Weaknesses
* It may have some security problems, since it is a shared database hosting [17][17].
* Backup Problems. For example, all the backups are on the Amazon's servers. It is difficult to backup locally.
* Maintance Window makes the database systems not accessible. [18][18] [19][19]

[14]: http://www.laurencegellert.com/2013/04/aws-benchmark-of-mysql-5-5-rds-vs-ec2/
[15]: http://getasysadmin.com/2011/02/mysql-benchmark-rds-ec2-performance/
[16]:https://aws.amazon.com/blogs/aws/amazon-rds-for-postgresql-now-available/
[17]: http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/
[18]:http://aws-musings.com/database-in-cloud-should-i-use-amazon-rds-or-mysql-installed-on-an-ebs-backed-ec2-instance/
[19]: http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBMaintenance.html
---

### StormDB
#### Strengths
* Powered by Postgres-XL, which is open-source. [20][20]
* Full support for subqueries, fuctions, triggers, ORMs, etc. [20][20]
* no virtualization, less overhead to operations [20][20]
* GIS support [20][20]

#### Weaknesses
* Lock on write, not MVCC

[20]: http://www.translattice.com/TransLattice_Storm.shtml
---
### SolidDB
####Strengths
* It is fast since it is a in-memory database system [21][21] [23][23] 
* Full ACID support [21][21] 
* Free [21][21]

####Weaknesses
* The weaknesses may be the same as the weaknesses of in-memory database system. 
	* For example, size of database is limited by size of main memory [22][22]. 
	* For another example, if the speed of the whole system depends on the performance of application, it is a waste of using in-memory dataplatform [24][24]. 
	* There are some other reasons why in-memory database have not taken the world [25][25] [26][26].

[21]: http://unicomsi.com/products/soliddb/
[22]: http://www.developerfeed.com/compare-disk-vs-memory-databases
[23]: http://en.wikipedia.org/wiki/In-memory_database
[24]: http://news.dice.com/2013/11/20/deflating-the-hype-over-in-memory-computing/
[25]: http://elasticube.blogspot.com/2010/09/in-memory-bi-is-not-future-its-past.html
[26]: http://kdrrecruitment.com/news-blog/why-in-memory-databases-havent-taken-over-the-world/
---
###Microsoft SQL Server/SQL Server PDW

####Strength
* In-memory technology (which is not mentioned on the map) for OLTP, BI [27][27] [29][29]
* Support for popular tools, such as Hive plug-in, SSAS, PowerPivot, Hive ODBC, etc. [28][28]
* For PDW, it offers **HDInsight** (on A5 region) Hadoop [28][28]
* For PDW, it combines software and hardware [28][28]
* MPP [28][28]
* Using SQL queries for traditional relational database and Hadoop database. [28][28]
* Smart Backups [28][28]
* Advanced security policy [30][30]

#### Weaknesses
* For PDW, some operations execute less slowly, such as insert operation [28][28]
* Server appliances for transactional applications are absence [31][31]
* Not support Linux [31][31]
* Restriction of clustered columnstore indexes [32][32]

[27]:http://searchsqlserver.techtarget.com/feature/In-memory-from-xVelocity-to-the-memory-optimized-columnstore-index
[28]:http://www.itpub.net/thread-1862842-1-1.html
[29]:http://searchsqlserver.techtarget.com/feature/How-to-improve-OLTP-with-SQL-Server-2014-In-Memory
[30]:http://searchsqlserver.techtarget.com/tip/SQL-Server-encryption-features-in-SQL-Server-2014
[31]:http://searchsqlserver.techtarget.com/news/2240222052/SQL-Server-2014-etches-itself-in-memory
[32]:http://searchsqlserver.techtarget.com/feature/SQL-Server-2014-columnstore-index-the-good-the-bad-and-the-clustered
- - -
###SAP HANA
####Strengths
* Column and row-based database engine depending on how to use data [33][33]
* Optimizing storage of data on disk [33][33] [34][34]
* Support for ABAP and Java [33][33]
* embedded lots of libraries [33][33]
* Not need to move data [35][35]

####Weaknesses
* Portability [36][36]
* VM problems [36][36]
* When you come to SAP HANA from traditional RDBMS, you need to pay more attention to some differences. [37][37] [38][38]
* Expensive


[33]:http://www.computereconomics.com/article.cfm?id=1732
[34]:http://www.davewentzel.com/content/sap-hana-evaluation
[35]:http://storage.chinabyte.com/345/12517845.shtml
[36]:http://www.searchbi.com.cn/showcontent_80652.htm
[37]:http://scn.sap.com/community/hana-in-memory/blog/2013/12/29/6-golden-rules-for-new-sap-hana-developers
[38]:http://scn.sap.com/community/hana-in-memory/blog/2014/04/02/why-sap-hana-has-not-had-more-success-than-it-deserves-no-i-do-not-work-for-sap

- - -
###IBM DB2/PureData 

####Strengths
* Support many features of SQL, compared with MS SQL Server [39][39]
* Support many platform [39][39]
* Self-Tuning Memory Management (STMM) [39][39]

#### Weaknesses
* Less robust than Oracle [40][40]
* Expensive [40][40]  
* Administration Required [40][40] 


[39]:http://www.ehow.com/info_12106599_advantages-db2.html
[40]:http://www.experts-exchange.com/Database/Miscellaneous/Q_20562672.html
- - -
###Oracle Database
####Strengths
* Much support resources
* Support multiple platforms
* Great Scalability
* Great Stability

####Weaknesses
* Expensive
* Administration Required
- - -
###MySQL
####Strengths
* Have many pluggable storage engines, which add lots of capabilities [41][41]
* Better technical choices for web applications [41][41]
* Inexpensive. Can be accessed with without license or permission [42][42]
* Very easy to use [42][42]
* Manages memory very well as it prevents memory leaks [43][43]

####Weaknesses
* Reluctant to accept patches from external sources [44][44]
* Security is vulnerable [45][45]
* Developing and debugging tools are relatively not so good [45][45]

[41]:http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/2
[42]:http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL
[43]:https://www.novell.com/documentation/nw65/web_mysql_nw/data/aj5bj52.html
[44]:http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing
[45]:http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL

- - -
### MySQL Cluster
####Strengths
* The system can work with inexpensive hardware. It has very small amounts of specific requirements for software as well. [46][46]
* Can combine multiple MySQL servers with the NDB (Network Database) storage engine [46][46]
* Can handle single point of failure as each component has independent memory and disk [46][46]

####Weaknesses
* There are issues in recovering memory usage. It cannot automatically recover used memory when data are deleted. [47][47]
* Inconvenient as MySQL Cluster Syntax cannot completely be compliant with SQL syntax [48][48]
* MySQL Cluster has some unsupported or missing features. [49][49] 

[46]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-overview.html
[47]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-limits.html
[48]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-transactions.html
[49]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-unsupported.html
- - -
### ￼MySQL Fabric
####Strengths
* High Availability. This includes automated failover and transparent failover. Automated failover means that MySQL Fabric prevents both reads and writes from stopping by automatically promoting ones of its slaves to be the new master when it detects the old master fails. In the process of changing a new master, the application is completely transparent, as it does not have to make any changes. [50][50] [51][51]
* Scaling. This includes using data partitioning and sharing. It automates the approach of scaling reads, which is adding more read slaves, and scaling writing, which is partitioning data into different shards. [50][50] [51][51]

####Weaknesses
* To the application, sharding is not completely transparent, as it has to provide the sharding key when accessing the database. [50][50]
* “Auto-increment columns cannot be used as a sharding key” [50][50]
* Has limitations on the scope of transactions and queries as it does not support too many rows in a single shard. [50][50]
* Must be restarted if fails. [50][50]

[50]:http://dev.mysql.com/tech-resources/articles/mysql-fabric-ga.html
[51]:http://www.mysql.com/products/enterprise/fabric/features.html

- - -
### PostgreSQL
####Strengths
* Strong security and safety feature [51][51]
* Have various types of stored procedure languages [51][51]
* Designed for high volume environments. Can handle much larger websites. [52][52]
* Open source [52][52]

####Weaknesses
* Lack of mature replication software. Need external solutions. [53][53]
* Inserting very long data is not allowed [54][54]

[51]:http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/1
[52]:http://www.postgresql.org/about/advantages/
[53]:http://www.anchor.com.au/hosting/dedicated/mysql_vs_postgres#head-0ca91f0bef42138084fa05a13d8ec1e4107d6dbd-2
[54]:http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing
- - -
### ScaleDB

####Strengths
* There is no need to partition data. [55][55]
* Lower Total Cost of Ownership (TCO), which includes software license costs, hardware costs, and development & maintenance costs. [56][56] 
* When the number of servers increases, the performance is still smooth. [57][57]
* Add adjust servers freely, and only need to pay for servers that actually use. [57][57]

####Weaknesses
* Lack of multi-version concurrency control (MVCC) support [58][58]
* Lack of complete geographic information system (GIS) support [58][58]

[55]:http://www.scaledb.com/resources/faq.php
[56]:http://scaledb.com/pdfs/WP_SDvSN.pdf
[57]:http://scaledb.com/pdfs/Overview_Datasheet.pdf
[58]:http://akelios.com/tools/scaledb
- - -
### SQLite
####Strengths
* Open source
* Compactness, very light
* Portability, File based [59][59]
* Easy developing and testing [59][59]
####Weaknesses
* No features for user management [59][59]
* Lack of space of Optimizing it to obtain extra performance [59][59]
* Locks whole file when writing
* Not scalable
* Restriction of size of database 

[59]:https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
- - -
### Splice Machine (Hadoop/New SQL DB)
####Strengths
* Hadoop scale-out technology [60][60]
* Do not need to rewrite applications because it support full ANSI SQL [60][60]
* low learning cost for who is familiar with RDBMS [60][60] [61][61]
* Fast [61][61]
####Weaknesses
* It is still on the initial stage

[60]:http://www.splicemachine.com/why-splice/
[61]:http://www.infoworld.com/article/2608217/hadoop/why-run-sql-on-nosql--speed--says-splice-machine.html
- - -
### MarkLogic (Search/Graph)
####Strengths
* support different kinds of data, such as XML, JSON, etc. [62][62] [65][65]
* document store [64][64]
* built-in search / sophisticated indexes technology [63][63] [65][65]
* RDF and SPARQL [66][66]
* Ability of connecting with Hadoop
####Weaknesses
* In some circumstances, data migration may be relatively hard. [67][67]
* Lack of libraries

[62]: http://www.marklogic.com/what-is-marklogic/
[63]:http://www.marklogic.com/what-is-marklogic/big-data-search/
[64]:http://developer.marklogic.com/blog/marklogic-beyond-nosql
[65]:http://stackoverflow.com/questions/545184/the-advantages-disadvantages-of-xml-compared-to-rdms
[66]:http://www.w3.org/2001/sw/wiki/SPARQL
[67]:http://www.odbms.org/blog/2012/10/two-cons-against-nosql-part-i/
[68]:http://www.odbms.org/blog/2012/11/two-cons-against-nosql-part-ii/
- - -
### OrientDB (General Purpose/Document/Graph)
####Strengths
* Fast
* Flexibility
* Zero-Configuration and Distributed Reliability
* Open source
* Support ACID, compared with MongoDB [70][70]
* SQL-like query language [70][70]
* Support different indexing algorithms, such as SB-Tree [70][70]
####Weaknesses
* On the other side, documentation is a limitation.

[69]:http://www.orientechnologies.com/why-orientdb/
[70]:http://www.orientechnologies.com/orientdb-vs-mongodb/
- - -
### Google Cloud Datastore(aaS/BigTable)
####Strengths
* bigTable [71][71]
####Weaknesses
* Not easy to understand and use [72][72]

[71]:http://static.googleusercontent.com/media/research.google.com/zh-CN/us/archive/bigtable-osdi06.pdf
- - -
### DataStax Enterprise(BigTable/Search/Key Value Stores/Hadoop)
####Strengths
####Weaknesses
- - -
### YarcData(Graph/Appliance/Specialist analytic)
####Strengths
####Weaknesses
- - -
### ObjectRocket Redis(aaS/In-memory/Key Value Stores)
####Strengths
####Weaknesses
- - -
### MemCachier
####Strengths
####Weaknesses
- - -
### Red Hat JBoss Data Grid
####Strengths
####Weaknesses
- - -
### GridGain
####Strengths
####Weaknesses
- - -

#### References
1. BigHadoop, 'Database.com - Salesforce.com's Cloud Database', 2013. [Online]. Available: https://bighadoop.wordpress.com/2013/10/14/database-com-salesforce-coms-cloud-database/. [Accessed: 24- Jan- 2015].
2. Salesforce.com, 'Database.com Workbook', 2015. [Online]. Available: http://www.salesforce.com/us/developer/docs/workbook_database/. [Accessed: 24- Jan- 2015].
3. E.Knorr, 'What Salesforce's Database.com really means', InfoWorld, 2015. [Online]. Available: http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html. [Accessed: 24- Jan- 2015].
4. Trust.salesforce.com, 'Security Best Practices – salesforce.com', 2015. [Online]. Available: https://trust.salesforce.com/trust/practices/. [Accessed: 24- Jan- 2015].
5. Salesforce.com, 'Salesforce1 Platform: Everything you need to build apps fast. - Salesforce.com', 2015. [Online]. Available: http://www.salesforce.com/platform/services/. [Accessed: 24- Jan- 2015].
6. Searchsqlserver.techtarget.com, 'Evolution of Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/essentialguide/Evolution-of-Windows-Azure-SQL-Database. [Accessed: 25- Jan- 2015].
7. Azure.microsoft.com, 'Cloud Services - SQL Database | Microsoft Azure', 2015. [Online]. Available: http://azure.microsoft.com/en-us/services/sql-database/. [Accessed: 25- Jan- 2015].
8. Wikipedia, 'SQL Azure', 2015. [Online]. Available: http://en.wikipedia.org/wiki/SQL_Azure. [Accessed: 25- Jan- 2015].
9. Searchsqlserver.techtarget.com, 'The pros of Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/The-pros-of-Windows-Azure-SQL-Database. [Accessed: 25- Jan- 2015].
10. Searchsqlserver.techtarget.com, 'Why you should think twice about Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/Why-you-should-think-twice-about-Windows-Azure-SQL-Database. [Accessed: 25- Jan- 2015].
11. Searchsqlserver.techtarget.com, 'SQL Azure security terrifies IT, but loss of control might be real fear', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/SQL-Azure-security-terrifies-IT-but-loss-of-control-might-be-real-fear. [Accessed: 25- Jan- 2015].
12. Cleardb.com, 'ClearDB -The Safer, Reliable MySQL Cloud Database For Your Applications', 2015. [Online]. Available: https://www.cleardb.com/better.view. [Accessed: 25- Jan- 2015].
13. Stackshare.io, 'Amazon RDS vs ClearDB vs Google Cloud SQL | StackShare', 2015. [Online]. Available: http://stackshare.io/stackups/amazon-rds-vs-cleardb-vs-google-cloud-sql. [Accessed: 25- Jan- 2015].
14. Laurencegellert.com, 'AWS benchmark of MySQL 5.5 RDS vs EC2 | Laurence Gellert's Blog', 2015. [Online]. Available: http://www.laurencegellert.com/2013/04/aws-benchmark-of-mysql-5-5-rds-vs-ec2/. [Accessed: 25- Jan- 2015].
15. Get A Sys Admin, 'Mysql benchmark: RDS vs EC2 performance - Get A Sys Admin', 2011. [Online]. Available: http://getasysadmin.com/2011/02/mysql-benchmark-rds-ec2-performance/. [Accessed: 25- Jan- 2015].
16. Aws.amazon.com, 'Amazon RDS for PostgreSQL â€“ Now Available | AWS Official Blog', 2015. [Online]. Available: https://aws.amazon.com/blogs/aws/amazon-rds-for-postgresql-now-available/. [Accessed: 25- Jan- 2015].
17. Laurencegellert.com, 'Pros and Cons of RDS vs EC2 for MySQL with AWS | Laurence Gellert's Blog', 2015. [Online]. Available: http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/. [Accessed: 25- Jan- 2015].
18. Aws-musings.com, 'Database in cloud â€“ Amazon RDS or MySQL on ebs? | My AWS Musings', 2010. [Online]. Available: http://aws-musings.com/database-in-cloud-should-i-use-amazon-rds-or-mysql-installed-on-an-ebs-backed-ec2-instance/. [Accessed: 25- Jan- 2015].
19. Docs.aws.amazon.com, 'Amazon RDS Maintenance Window - Amazon Relational Database Service', 2015. [Online]. Available: http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBMaintenance.html. [Accessed: 25- Jan- 2015].







