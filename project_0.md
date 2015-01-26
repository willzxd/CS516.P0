# Project 0
Xiaodan Zhu
<br />Date: Jan 25, 2015
<br />Version: 1.0
<br />

Project requirement:<br />
For every single system listed in the “DataPlatformsMap”, give as a list of succinct points:*  Strengths (with numbered references)*  Weaknesses (with numbered references)*  References (can be articles, blog posts, research papers, white papers, your own assessment, ...)

===
=== 
## Introduction
I try to trace different routines mentioned on this map. And I am more interested in what I have never heard.

===
===

## Analysis of dataplatforms
===

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


#### Weaknesses
* It is not perform well, if some company want to build a data-intensive system by using Database.com. Internet latency is a big problem.[3][3]
* I doubt the security of this platform becasue it only combine lots of regular policy together. There are no advanced technology to prove that it is "the world's most trusted and secure cloud database" [4][4].
* The website terribly works in Safari [5][5]. If a company cannot properly show the contents of website, it is difficult for me to trust its products.



===
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

#### Weaknesses
* Lots of T-SQL features do not be implemented [10][10]
* Extra charge [10][10]
* Security Probems [11][11] (For example, it does not support encrypting transparent data [10][10].) 

===
### ClearDB
* DaaS
* Part of MySQL ecosystem

#### Strengths
* Geo distributed cloud database system[12][12]
* Safety (Backup globally)[12][12]
* That Database is next to applications eliminates latency issuses.[12][12]


#### Weakneeses
* Features is not many as some other DaaS.[13][13]


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

---

### StormDB
#### Strengths
* Powered by Postgres-XL, which is open-source. [20][20]
* Full support for subqueries, fuctions, triggers, ORMs, etc. [20][20]
* no virtualization, less overhead to operations [20][20]
* GIS support [20][20]

#### Weaknesses
* Lock on write, not MVCC


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

---
###Microsoft SQL Server/SQL Server PDW

####Strengths
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

===
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

===
###Informix
####Strengths
* Integrating SQL, NoSQL/JSON, etc. [39][39]
* ACID support [39][39]
* Easy administration [39][39]
* In-memory, column-based technology [39][39]
####Weaknesses
* Not scalable
* Consistency

===
###IBM DB2/PureData 

####Strengths
* Support many features of SQL, compared with MS SQL Server [40][40]
* Support many platform [40][40]
* Self-Tuning Memory Management (STMM) [40][40]

#### Weaknesses
* Less robust than Oracle [41][41]
* Expensive [41][41]  
* Administration Required [41][41] 

===
###Oracle Database
####Strengths
* Much support resources
* Support multiple platforms
* Great Scalability
* Great Stability

####Weaknesses
* Expensive
* Administration Required

===
###Oracle Exadata
####Strength
* High performance
* Scale-out architecture

####Weaknesses
* Expensive

===
### Oracle Exalytics
####Strengths
* Part of Oracle database ecosystem [42][42]
* In-memory [42][42]

####Weaknesses
* Restriction of database size
* Expensive

===
###XtremeData
####Strengths
* ANSI SQL
* Easy deployment[43][43]
####Weaknesses
* weak support for OLTP

===

### Teradata
####Strengths
* high performance for high workloads[44][44]
* indexing, partitioning, in-memory and column-based technology[44][44]

####Weaknesses
* Expensive [44][44]


===
###SQream

####Strengths
* High performance for analysis and transaction
* GPU-based technology[45][45]

===
###SciDB
####Strengths
* ACID [46][46]
* R and Python [46][46]
* Shared-nothing [46][46]

####Weakness
* Not support SQL language [46][46]

===
###MySQL
####Strengths
* Have many pluggable storage engines, which add lots of capabilities [47][47]
* Better technical choices for web applications [47][47]
* Inexpensive. Can be accessed with without license or permission [48][48]
* Very easy to use [48][48]
* Manages memory very well as it prevents memory leaks [49][49]

####Weaknesses
* Reluctant to accept patches from external sources [50][50]
* Security is vulnerable [51][51]
* Developing and debugging tools are relatively not so good [51][51]

===
### MySQL Cluster
####Strengths
* The system can work with inexpensive hardware. It has very small amounts of specific requirements for software as well. [52][52]
* Can combine multiple MySQL servers with the NDB (Network Database) storage engine [52][52]
* Can handle single point of failure as each component has independent memory and disk [53][53]

####Weaknesses
* There are issues in recovering memory usage. It cannot automatically recover used memory when data are deleted. [53][53]
* Inconvenient as MySQL Cluster Syntax cannot completely be compliant with SQL syntax [54][54]
* MySQL Cluster has some unsupported or missing features. [55][55] 

===
### ￼MySQL Fabric
####Strengths
* High Availability. This includes automated failover and transparent failover. Automated failover means that MySQL Fabric prevents both reads and writes from stopping by automatically promoting ones of its slaves to be the new master when it detects the old master fails. In the process of changing a new master, the application is completely transparent, as it does not have to make any changes. [56][56] [57][57]
* Scaling. This includes using data partitioning and sharing. It automates the approach of scaling reads, which is adding more read slaves, and scaling writing, which is partitioning data into different shards.[56][56] [57][57]

####Weaknesses
* To the application, sharding is not completely transparent, as it has to provide the sharding key when accessing the database. [56][56]
* “Auto-increment columns cannot be used as a sharding key” [56][56]
* Has limitations on the scope of transactions and queries as it does not support too many rows in a single shard. [56][56]
* Must be restarted if fails. [56][56]

===
### PostgreSQL
####Strengths
* Strong security and safety feature [58][58]
* Have various types of stored procedure languages [58][58]
* Designed for high volume environments. Can handle much larger websites. [59][59]
* Open source [59][59]

####Weaknesses
* Lack of mature replication software. Need external solutions. [60][60]
* Inserting very long data is not allowed [61][61]

===
### ScaleDB

####Strengths
* There is no need to partition data. [62][62]
* Lower Total Cost of Ownership (TCO), which includes software license costs, hardware costs, and development & maintenance costs. [63][63] 
* When the number of servers increases, the performance is still smooth. [64][64]
* Add adjust servers freely, and only need to pay for servers that actually use. [64][64]

####Weaknesses
* Lack of multi-version concurrency control (MVCC) support [65][65]
* Lack of complete geographic information system (GIS) support [65][65]


===
### SQLite
####Strengths
* Open source
* Compactness, very light
* Portability, File based [66][66]
* Easy developing and testing [66][66]
####Weaknesses
* No features for user management [66][66]
* Lack of space of Optimizing it to obtain extra performance [66][66]
* Locks whole file when writing
* Not scalable
* Restriction of size of database 

===
### Splice Machine (Hadoop/New SQL DB)
####Strengths
* Hadoop scale-out technology [67][67]
* Do not need to rewrite applications because it support full ANSI SQL [67][67]
* low learning cost for who is familiar with RDBMS  [67][67] [68][68]
* Fast [68][68]
####Weaknesses
* It is still on the initial stage


===
### MarkLogic (Search/Graph)
####Strengths
* support different kinds of data, such as XML, JSON, etc. [69][69] [72][72]
* document store [71][71]
* built-in search / sophisticated indexes technology [70][70] [72][72]
* RDF and SPARQL [73][73]
* Ability of connecting with Hadoop
####Weaknesses
* In some circumstances, data migration may be relatively hard. [74][74] [75][75]
* Lack of libraries

===
### OrientDB (General Purpose/Document/Graph)
####Strengths
* Fast
* Flexibility
* Zero-Configuration and Distributed Reliability
* Open source
* Support ACID, compared with MongoDB [76][76]
* SQL-like query language [76][76]
* Support different indexing algorithms, such as SB-Tree [77][77]
####Weaknesses
* On the other side, documentation is a limitation.

===
### Google Cloud Datastore(aaS/BigTable)
####Strengths
* BigTable [78][78]
 	* High availability
 	* High consistency
 	* Hight availability
 	
####Weaknesses
* Not easy to understand and use [79][79]
* No Join operation

===
###HBase 
[83][83]

####Strengths [k][k]

* Combination of Bigtable, Hadoop and HDFS [80][80] [81][81]
* Good for real time queries
* optimizing for batch inserts, updates, and deletes, consistent reads and writes [82][82]

####Weakness
* weak support for ACID
* No Join operation

===
###Accumulo

####Strengths [84][84]
* Bigtable on top of Hadoop and HDFS;
* Cell-level security[l][l]

####Weakness
* master-slave architecture;
* weak support for ACID
* No Join operation

===
###Riak
####Strengths
* Open source [85][85]
* Low-Latency [85][85]
* Fault-Tolerance [85][85]
* eventually consistent system [86][86]

####Weaknesses
* overkill for small databases 
* only support key-value as its atomic elements  [86][86]
* not efficient for high query workload  [86][86]
* Not support for SQL-like language
* Not support ACID
* Not support Join operation


===
###Cassandra
####Strengths
* Elastic scalability [87][87]
* Fast linear-scale performance [87][87]
* Flexible data storage  [87][87]
* Transaction support [87][87]

####Weaknesses
* Sub-millisecond consistency [88][88]
* Transactions [88][88]
* Ad-hoc querying [88][88]
* Consistent indexes on values [88][88]
* consistent read/write latency of heavy load [88][88]

===
### DataStax Enterprise(BigTable/Search/Key Value Stores/Hadoop)
####Strengths
* continuous availability
* fast performance
* strong security

####Weaknesses
* limitation of in-memory tables



===

### Redis
####Strengths
* Fast
* concurrency support
* In-memory key-value store
* Higher availability by using master-slave replication
* Optimizing locks
* Persistence to disk
* Scalable as a cache

####Weaknesses
* Immature [89][89]
* limitation of memory [89][89]
* Scalability [89][89]

===
### ObjectRocket Redis(aaS/In-memory/Key Value Stores)
almost the same as Redis

===
###AWS ElastiCache, AWS ElastiCache with Redis
####Strength

* Simply deploy and manage [90][90]
* Elasticity and scalability [90][90]
* Failure detection and recovery [90][90]
* Part of AWS [90][90]

####Weakness
* Consistency

===
###RedisLabs Memcached Cloud

####Strength

* Reliability
* Backup/FTP
* Better Elasticity and scalability

===
###RedisLabs Redis Cloud

####Strength
almost same as above

===
### MemCachier
####Strengths
* Dashboard for monitoring

===

### Red Hat JBoss Data Grid
####Strengths
* In-memory [91][91] [92][92]
* Fast [91][91]
* Schema-less
* Scalable
* Fault tolerance
* Concurrency control with multiversions
* Support different strategies for persistent storage [93][93]
####Weaknesses
* difficult for Migrating from SQL
* Network bandwidth may have a great influence
* more validation should be implement on applications

===
###Infinispan
####Strengths
* In-memory [~][~] [?][?]
* Fast [~][~]
* Schema-less
* Scalable
* Fault tolerance
* Concurrency control with multiversions
* Support different strategies for persistent storage [P][P]
####Weaknesses
* difficult for Migrating from SQL
* Network bandwidth may have a great influence
* more validation should be implement on applications

===

### GridGain
####Strengths
* In-Memory MapReduce
* Low latency
* Scalable
* Multiversion concurrency control
* Schema-less

####Weaknesses
* same as a grid database

===
###Apache Storm

####Strengths

* Processing large streaming events [94][94]
* Compatibility [94][94]
* Scalability[94][94]
* Fault tolerance [94][94]
* Easy-use API[94][94]

####Weaknesses
* weak framework [95][95]



===
###SQLStream

####Strengths

* Real-time stream processing
* low latency
* SQL for stream processing [96][96]

####Weaknesses
* SQL queries may cause problems

===

###DataTorrent

####Strengths

* Real-time stream processing with Hadoop
* Built-in fault-tolerance [97][97]

===
###Amazon Kinesis

####Strengths

* Full-managed real-time stream processing platform with support
* Elastic scalability
* Part of Amazon services
* built-in monitor

===
###Google Cloud Dataflow

####Strengths

* real-time stream processing
* scalability
* Part of Google services [98][98]

####Weaknesses
* Still on the way [98][98] [99][99]

===
###SRCH2(Search towards enterprise Search)
####Strengths
* Full text in-memory index [100][100]
* built wit C++ [100][100]
* restful API [100][100]
* Powerful search functions[100][100]
* Support for global language [100][100]
* Record-based access-control lists (ACL) [101][101]

####Weaknesses
* Only a search engine
* Need to connect to other database systems [102][102]


===
###Loggly (Search Towards SIEM)
A security information and event management (SIEM) product

####Strengths
* Responsive Log Management™ [103][103]

####Weaknesses
* Can't help too much find infrastructure, security or analytics solutions [104][104]



<br />

[1]: https://bighadoop.wordpress.com/2013/10/14/database-com-salesforce-coms-cloud-database/
[2]: http://www.salesforce.com/us/developer/docs/workbook_database/
[3]: http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html
[4]:https://trust.salesforce.com/trust/practices/
[5]: http://www.salesforce.com/platform/services/
[6]: http://searchsqlserver.techtarget.com/essentialguide/Evolution-of-Windows-Azure-SQL-Database
[7]: http://azure.microsoft.com/en-us/services/sql-database/
[8]: http://en.wikipedia.org/wiki/SQL_Azure
[9]: http://searchsqlserver.techtarget.com/feature/The-pros-of-Windows-Azure-SQL-Database
[10]: http://searchsqlserver.techtarget.com/feature/Why-you-should-think-twice-about-Windows-Azure-SQL-Database
[11]: http://searchsqlserver.techtarget.com/feature/SQL-Azure-security-terrifies-IT-but-loss-of-control-might-be-real-fear 
[12]:https://www.cleardb.com/better.view
[13]:http://stackshare.io/stackups/amazon-rds-vs-cleardb-vs-google-cloud-sql
[14]: http://www.laurencegellert.com/2013/04/aws-benchmark-of-mysql-5-5-rds-vs-ec2/
[15]: http://getasysadmin.com/2011/02/mysql-benchmark-rds-ec2-performance/
[16]:https://aws.amazon.com/blogs/aws/amazon-rds-for-postgresql-now-available/
[17]: http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/
[18]:http://aws-musings.com/database-in-cloud-should-i-use-amazon-rds-or-mysql-installed-on-an-ebs-backed-ec2-instance/
[19]: http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBMaintenance.html
[20]: http://www.translattice.com/TransLattice_Storm.shtml
[21]: http://unicomsi.com/products/soliddb/
[22]: http://www.developerfeed.com/compare-disk-vs-memory-databases
[23]: http://en.wikipedia.org/wiki/In-memory_database
[24]: http://news.dice.com/2013/11/20/deflating-the-hype-over-in-memory-computing/
[25]: http://elasticube.blogspot.com/2010/09/in-memory-bi-is-not-future-its-past.html
[26]: http://kdrrecruitment.com/news-blog/why-in-memory-databases-havent-taken-over-the-world/
[27]:http://searchsqlserver.techtarget.com/feature/In-memory-from-xVelocity-to-the-memory-optimized-columnstore-index
[28]:http://www.itpub.net/thread-1862842-1-1.html
[29]:http://searchsqlserver.techtarget.com/feature/How-to-improve-OLTP-with-SQL-Server-2014-In-Memory
[30]:http://searchsqlserver.techtarget.com/tip/SQL-Server-encryption-features-in-SQL-Server-2014
[31]:http://searchsqlserver.techtarget.com/news/2240222052/SQL-Server-2014-etches-itself-in-memory
[32]:http://searchsqlserver.techtarget.com/feature/SQL-Server-2014-columnstore-index-the-good-the-bad-and-the-clustered
[33]:http://www.computereconomics.com/article.cfm?id=1732
[34]:http://www.davewentzel.com/content/sap-hana-evaluation
[35]:http://storage.chinabyte.com/345/12517845.shtml
[36]:http://www.searchbi.com.cn/showcontent_80652.htm
[37]:http://scn.sap.com/community/hana-in-memory/blog/2013/12/29/6-golden-rules-for-new-sap-hana-developers
[38]:http://scn.sap.com/community/hana-in-memory/blog/2014/04/02/why-sap-hana-has-not-had-more-success-than-it-deserves-no-i-do-not-work-for-sap
[39]:http://www-01.ibm.com/support/docview.wss?uid=swg27019520
[40]:http://www.ehow.com/info_12106599_advantages-db2.html
[41]:http://www.experts-exchange.com/Database/Miscellaneous/Q_20562672.html
[42]:https://www.oracle.com/engineered-systems/exalytics/index.html
[43]:http://architects.dzone.com/articles/large-scale-data-analytics
[44]:http://www.teradata.com/?LangType=1033&LangSelect=true
[45]:http://sqream.com/
[46]:http://www.paradigm4.com/technology/
[47]:http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/2
[48]:http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL
[49]:https://www.novell.com/documentation/nw65/web_mysql_nw/data/aj5bj52.html
[50]:http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing
[51]:http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL
[52]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-overview.html
[53]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-limits.html
[54]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-transactions.html
[55]:http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-unsupported.html
[56]:http://dev.mysql.com/tech-resources/articles/mysql-fabric-ga.html
[57]:http://www.mysql.com/products/enterprise/fabric/features.html
[58]:http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/1
[59]:http://www.postgresql.org/about/advantages/
[60]:http://www.anchor.com.au/hosting/dedicated/mysql_vs_postgres#head-0ca91f0bef42138084fa05a13d8ec1e4107d6dbd-2
[61]:http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing
[62]:http://www.scaledb.com/resources/faq.php
[63]:http://scaledb.com/pdfs/WP_SDvSN.pdf
[64]:http://scaledb.com/pdfs/Overview_Datasheet.pdf
[65]:http://akelios.com/tools/scaledb
[66]:https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
[67]:http://www.splicemachine.com/why-splice/
[68]:http://www.infoworld.com/article/2608217/hadoop/why-run-sql-on-nosql--speed--says-splice-machine.html
[69]: http://www.marklogic.com/what-is-marklogic/
[70]:http://www.marklogic.com/what-is-marklogic/big-data-search/
[71]:http://developer.marklogic.com/blog/marklogic-beyond-nosql
[72]:http://stackoverflow.com/questions/545184/the-advantages-disadvantages-of-xml-compared-to-rdms
[73]:http://www.w3.org/2001/sw/wiki/SPARQL
[74]:http://www.odbms.org/blog/2012/10/two-cons-against-nosql-part-i/
[75]:http://www.odbms.org/blog/2012/11/two-cons-against-nosql-part-ii/
[76]:http://www.orientechnologies.com/why-orientdb/
[77]:http://www.orientechnologies.com/orientdb-vs-mongodb/
[78]:http://static.googleusercontent.com/media/research.google.com/zh-CN/us/archive/bigtable-osdi06.pdf
[79]:http://www.codeproject.com/Articles/716717/Google-Cloud-Datastore
[80]:https://haifengl.wordpress.com/2014/05/14/hbase-and-accumulo/
[81]:http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
[82]:http://hbase.apache.org/book.html#arch.hdfs
[83]:http://hbase.apache.org/
[84]:http://wikibon.org/blog/breaking-analysis-accumulo-why-the-world-needs-another-nosql-database/
[85]:http://basho.com/riak
[86]:http://docs.basho.com/riak/latest/theory/why-riak/
[87]:http://www.datastax.com/what-we-offer/products-services/datastax-enterprise/apache-cassandra
[88]:http://www.quora.com/What-are-the-main-disadvantages-of-using-cassandra-what-are-the-scenarios-where-cassandra-should-not-be-my-first-selection
[89]:http://stackoverflow.com/questions/10906246/what-is-the-disadvantage-of-just-using-redis-instead-of-an-rdbms
[90]:http://aws.amazon.com/cn/documentation/elasticache/
[91]:http://www.slideshare.net/galderz/data-grids-vs-databases
[92]:http://www.slideshare.net/galderz/data-grids-and-data-caching
[93]:https://access.redhat.com/documentation/en-US/Red_Hat_JBoss_Data_Grid/6.4/pdf/Getting_Started_Guide/Red_Hat_JBoss_Data_Grid-6.4-Getting_Started_Guide-en-US.pdf
[94]: https://storm.apache.org/documentation/Rationale.html
[95]: http://www.infoq.com/articles/stream-processing-hadoop
[96]: http://www.sqlstream.com/stream-processing-with-sql/
[97]:http://www.datanami.com/2014/04/23/crossing_the_big_data_stream_with_datatorrent/
[98]:http://venturebeat.com/2014/06/25/google-cloud-dataflow/
[99]:http://static.googleusercontent.com/media/research.google.com/en/us/archive/mapreduce-osdi04.pdf
[100]:http://srch2.com/products/
[101]:http://srch2.com/srch2-introduces-access-control-lists-improve-search-security/
[102]:http://srch2.com/releases/4.4.3/docs/
[103]:https://www.loggly.com/why-loggly/
[104]:http://blog.takipi.com/the-7-log-management-tools-you-need-to-know/

======

### References
[1] BigHadoop, 'Database.com - Salesforce.com's Cloud Database', 2013. [Online]. Available: https://bighadoop.wordpress.com/2013/10/14/database-com-salesforce-coms-cloud-database/. [Accessed: 26- Jan- 2015].
<br />[2] Salesforce.com, 'Database.com Workbook', 2015. [Online]. Available: http://www.salesforce.com/us/developer/docs/workbook_database/. [Accessed: 26- Jan- 2015].
<br />[3]E.  Knorr, 'What Salesforce's Database.com really means', InfoWorld, 2015. [Online]. Available: http://www.infoworld.com/article/2624989/cloud-computing/what-salesforce-s-database-com-really-means.html. [Accessed: 26- Jan- 2015].
<br />[4] Trust.salesforce.com, 'Security Best Practices â€“ salesforce.com', 2015. [Online]. Available: https://trust.salesforce.com/trust/practices/. [Accessed: 26- Jan- 2015].
<br />[5] Salesforce.com, 'Salesforce1Â Platform: Everything you need to build apps fast. - Salesforce.com', 2015. [Online]. Available: http://www.salesforce.com/platform/services/. [Accessed: 26- Jan- 2015].
<br />[6] Searchsqlserver.techtarget.com, 'Evolution of Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/essentialguide/Evolution-of-Windows-Azure-SQL-Database. [Accessed: 26- Jan- 2015].
<br />[7] Azure.microsoft.com, 'Cloud Services - SQL Database | Microsoft Azure', 2015. [Online]. Available: http://azure.microsoft.com/en-us/services/sql-database/. [Accessed: 26- Jan- 2015].
<br />[8] Wikipedia, 'SQL Azure', 2015. [Online]. Available: http://en.wikipedia.org/wiki/SQL_Azure. [Accessed: 26- Jan- 2015].
<br />[9] Searchsqlserver.techtarget.com, 'The pros of Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/The-pros-of-Windows-Azure-SQL-Database. [Accessed: 26- Jan- 2015].
<br />[10] Searchsqlserver.techtarget.com, 'Why you should think twice about Windows Azure SQL Database', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/Why-you-should-think-twice-about-Windows-Azure-SQL-Database. [Accessed: 26- Jan- 2015].
<br />[11] Searchsqlserver.techtarget.com, 'SQL Azure security terrifies IT, but loss of control might be real fear', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/SQL-Azure-security-terrifies-IT-but-loss-of-control-might-be-real-fear. [Accessed: 26- Jan- 2015].
<br />[12]2015. .
<br />[13] Stackshare.io, 'Amazon RDS vs ClearDB vs Google Cloud SQL | StackShare', 2015. [Online]. Available: http://stackshare.io/stackups/amazon-rds-vs-cleardb-vs-google-cloud-sql. [Accessed: 26- Jan- 2015].
<br />[14] Laurencegellert.com, 'AWS benchmark of MySQL 5.5 RDS vs EC2 | Laurence Gellert's Blog', 2015. [Online]. Available: http://www.laurencegellert.com/2013/04/aws-benchmark-of-mysql-5-5-rds-vs-ec2/. [Accessed: 26- Jan- 2015].
<br />[15]2015. .
<br />[16] Aws.amazon.com, 'Amazon RDS for PostgreSQL â€“ Now Available | AWS Official Blog', 2015. [Online]. Available: https://aws.amazon.com/blogs/aws/amazon-rds-for-postgresql-now-available/. [Accessed: 26- Jan- 2015].
<br />[17] Laurencegellert.com, 'Pros and Cons of RDS vs EC2 for MySQL with AWS | Laurence Gellert's Blog', 2015. [Online]. Available: http://www.laurencegellert.com/2013/05/pros-and-cons-of-rds-vs-ec2-for-mysql-with-aws/. [Accessed: 26- Jan- 2015].
<br />[18] Aws-musings.com, 'Database in cloud â€“ Amazon RDS or MySQL on ebs? | My AWS Musings', 2010. [Online]. Available: http://aws-musings.com/database-in-cloud-should-i-use-amazon-rds-or-mysql-installed-on-an-ebs-backed-ec2-instance/. [Accessed: 26- Jan- 2015].
<br />[19] Docs.aws.amazon.com, 'Amazon RDS Maintenance Window - Amazon Relational Database Service', 2015. [Online]. Available: http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBMaintenance.html. [Accessed: 26- Jan- 2015].
<br />[20] Translattice.com, 'TransLattice Storm', 2015. [Online]. Available: http://www.translattice.com/TransLattice_Storm.shtml. [Accessed: 26- Jan- 2015].
<br />[21] Unicomsi.com, 'UNICOM Systems, Inc. -- A Division of UNICOM Global :: SolidDB', 2015. [Online]. Available: http://unicomsi.com/products/soliddb/. [Accessed: 26- Jan- 2015].
<br />[22] Developerfeed.com, 'Compare On-Disk v/s In-Memory Databases | DeveloperFeed', 2015. [Online]. Available: http://www.developerfeed.com/compare-disk-vs-memory-databases. [Accessed: 26- Jan- 2015].
<br />[23] Wikipedia, 'In-memory database', 2015. [Online]. Available: http://en.wikipedia.org/wiki/In-memory_database. [Accessed: 26- Jan- 2015].
<br />[24]M.  Matsumura, 'Deflating the Hype Over In-Memory Databases - Dice News', Dice News, 2013. [Online]. Available: http://news.dice.com/2013/11/20/deflating-the-hype-over-in-memory-computing/. [Accessed: 26- Jan- 2015].
<br />[25] Elasticube.blogspot.com, 'In-memory BI is not the future. Itâ€™s the past. - The ElastiCube Chronicles', 2010. [Online]. Available: http://elasticube.blogspot.com/2010/09/in-memory-bi-is-not-future-its-past.html. [Accessed: 26- Jan- 2015].
<br />[26] Kdrrecruitment.com, 'Why In-Memory Databases havenâ€™t taken over the world by Matthew Napleton Blog Post by KDR Recruitment', 2015. [Online]. Available: http://kdrrecruitment.com/news-blog/why-in-memory-databases-havent-taken-over-the-world/. [Accessed: 26- Jan- 2015].
<br />
[27] Searchsqlserver.techtarget.com, 'In-memory from xVelocity to the memory-optimized columnstore index', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/In-memory-from-xVelocity-to-the-memory-optimized-columnstore-index. [Accessed: 26- Jan- 2015].
<br />[28] Itpub.net, 'SQL Server 2014? - MS SQL Server-ITPUB', 2015. [Online]. Available: http://www.itpub.net/thread-1862842-1-1.html. [Accessed: 26- Jan- 2015].
<br />[29] Searchsqlserver.techtarget.com, 'How to improve OLTP with SQL Server 2014 In-Memory', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/How-to-improve-OLTP-with-SQL-Server-2014-In-Memory. [Accessed: 26- Jan- 2015].
<br />[30] Searchsqlserver.techtarget.com, 'SQL Server encryption features in SQL Server 2014', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/tip/SQL-Server-encryption-features-in-SQL-Server-2014. [Accessed: 26- Jan- 2015].
<br />[31] Searchsqlserver.techtarget.com, 'SQL Server 2014 etches itself in-memory', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/news/2240222052/SQL-Server-2014-etches-itself-in-memory. [Accessed: 26- Jan- 2015].
<br />[32] Searchsqlserver.techtarget.com, 'SQL Server 2014 columnstore index: the good, the bad and the clustered', 2015. [Online]. Available: http://searchsqlserver.techtarget.com/feature/SQL-Server-2014-columnstore-index-the-good-the-bad-and-the-clustered. [Accessed: 26- Jan- 2015].
<br />[33] Computereconomics.com, 'Is it Time to Switch to SAP HANA?', 2015. [Online]. Available: http://www.computereconomics.com/article.cfm?id=1732. [Accessed: 26- Jan- 2015].
<br />[34] Davewentzel.com, 'SAP HANA Evaluation | DaveWentzel.com', 2015. [Online]. Available: http://www.davewentzel.com/content/sap-hana-evaluation. [Accessed: 26- Jan- 2015].
<br />[35] Storage.chinabyte.com, 'SAP HANAï¿½ï¿½×¹ï¿½ï¿½ï¿½Exalyticsï¿½ï¿½Ò»ï¿½ï¿½ï¿½ï¿½ï¿½ï¿½Ê¦ï¿½Ä¿ï¿½ï¿½ï¿½_ï¿½æ´¢_ï¿½ï¿½ï¿½ï¿½ï¿½ï¿½', 2013. [Online]. Available: http://storage.chinabyte.com/345/12517845.shtml. [Accessed: 26- Jan- 2015].
<br />[36] Searchbi.com.cn, 'SAP BIå·¥å…·çš„ä¼˜ç¼ºç‚¹ - SAP - TechTargetå•†åŠ¡æ™ºèƒ½', 2015. [Online]. Available: http://www.searchbi.com.cn/showcontent_80652.htm. [Accessed: 26- Jan- 2015].
<br />[37] Scn.sap.com, '6 Golden Rules for New SAP HANA Developers', 2015. [Online]. Available: http://scn.sap.com/community/hana-in-memory/blog/2013/12/29/6-golden-rules-for-new-sap-hana-developers. [Accessed: 26- Jan- 2015].
<br />[38] Scn.sap.com, 'Why SAP HANA has not had more success than it deserves (no, I do not work for SAP)', 2015. [Online]. Available: http://scn.sap.com/community/hana-in-memory/blog/2014/04/02/why-sap-hana-has-not-had-more-success-than-it-deserves-no-i-do-not-work-for-sap. [Accessed: 26- Jan- 2015].
<br />[39] Www-01.ibm.com, 'IBM Publications for the IBM Informix 11.70 family of products - United States', 2015. [Online]. Available: http://www-01.ibm.com/support/docview.wss?uid=swg27019520. [Accessed: 26- Jan- 2015].
<br />[40]A.  Hughes, 'The Advantages of DB2 | eHow', eHow, 2015. [Online]. Available: http://www.ehow.com/info_12106599_advantages-db2.html. [Accessed: 26- Jan- 2015].
<br />[41] Experts-exchange.com, 'My SQL, SQL Server, DB2, Oracle Advantages Disadvantages?', 2003. [Online]. Available: http://www.experts-exchange.com/Database/Miscellaneous/Q_20562672.html. [Accessed: 26- Jan- 2015].
<br />[42] Oracle.com, 'Exalytics In-Memory Machine | Oracle', 2015. [Online]. Available: https://www.oracle.com/engineered-systems/exalytics/index.html. [Accessed: 26- Jan- 2015].
<br />[43] Architects.dzone.com, 'Large Scale Data Analytics with XtremeData Parallel SQL Database Engine | Architects Zone', 2015. [Online]. Available: http://architects.dzone.com/articles/large-scale-data-analytics. [Accessed: 26- Jan- 2015].
<br />[44] Teradata.com, 'Global Leader in Data Warehousing, Big Data Analytics & Data Driven Marketing - Teradata', 2015. [Online]. Available: http://www.teradata.com/?LangType=1033&LangSelect=true. [Accessed: 26- Jan- 2015].
<br />[45] SQream, 'HOME - SQream', 2015. [Online]. Available: http://sqream.com/. [Accessed: 26- Jan- 2015].
<br />[46] Paradigm4, 'Technology - Paradigm4', 2015. [Online]. Available: http://www.paradigm4.com/technology/. [Accessed: 26- Jan- 2015].
<br />[47] Eweek.com, 'MySQL Features and Functionality', 2015. [Online]. Available: http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/2. [Accessed: 26- Jan- 2015].
<br />[48]O.  Solutions, 'Advantages and Disadvantages of MySQL', HubPages, 2015. [Online]. Available: http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL. [Accessed: 26- Jan- 2015].
<br />[49] Novell.com, 'Novell Doc: NW 6.5 SP8: Novell MySQL Administration Guide - Benefits of MySQL', 2015. [Online]. Available: https://www.novell.com/documentation/nw65/web_mysql_nw/data/aj5bj52.html. [Accessed: 26- Jan- 2015].
<br />[50] Wikivs.com, 'MySQL vs PostgreSQL - WikiVS', 2015. [Online]. Available: http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing. [Accessed: 26- Jan- 2015].
<br />[51]O.  Solutions, 'Advantages and Disadvantages of MySQL', HubPages, 2015. [Online]. Available: http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL. [Accessed: 26- Jan- 2015].
<br />[52] Dev.mysql.com, 'MySQL ::   MySQL 5.1 Reference Manual :: 17.1 MySQL Cluster Overview', 2015. [Online]. Available: http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-overview.html. [Accessed: 26- Jan- 2015].
<br />[53] Dev.mysql.com, 'MySQL ::   MySQL 5.1 Reference Manual :: 17.1.6.2 Limits and Differences of MySQL Cluster from Standard MySQL Limits', 2015. [Online]. Available: http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-limits.html. [Accessed: 26- Jan- 2015].
<br />[54] Dev.mysql.com, 'MySQL ::   MySQL 5.1 Reference Manual :: 17.1.6.3 Limits Relating to Transaction Handling in MySQL Cluster', 2015. [Online]. Available: http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-transactions.html. [Accessed: 26- Jan- 2015].
<br />[55] Dev.mysql.com, 'MySQL ::   MySQL 5.1 Reference Manual :: 17.1.6.6 Unsupported or Missing Features in MySQL Cluster', 2015. [Online]. Available: http://dev.mysql.com/doc/refman/5.1/en/mysql-cluster-limitations-unsupported.html. [Accessed: 26- Jan- 2015].
<br />[56] Dev.mysql.com, 'MySQL ::  MySQL Fabric GA - Adding High Availability and/or Scaling to MySQL', 2015. [Online]. Available: http://dev.mysql.com/tech-resources/articles/mysql-fabric-ga.html. [Accessed: 26- Jan- 2015].
<br />[57] Mysql.com, 'MySQL ::  MySQL Fabric Features and Benefits', 2015. [Online]. Available: http://www.mysql.com/products/enterprise/fabric/features.html. [Accessed: 26- Jan- 2015].
<br />[58] Eweek.com, 'PostgreSQL Features and Functionality', 2015. [Online]. Available: http://www.eweek.com/c/a/Linux-and-Open-Source/PostgreSQL-vs-MySQL-How-to-Select-the-Right-OpenSource-Database/1. [Accessed: 26- Jan- 2015].
<br />[59] Postgresql.org, 'PostgreSQL: Advantages', 2015. [Online]. Available: http://www.postgresql.org/about/advantages/. [Accessed: 26- Jan- 2015].
<br />[60] Anchor.com.au, 'MySQL vs PostgreSQL comparison - Web and dedicated hosting tutorials by Anchor', 2015. [Online]. Available: http://www.anchor.com.au/hosting/dedicated/mysql_vs_postgres#head-0ca91f0bef42138084fa05a13d8ec1e4107d6dbd-2. [Accessed: 26- Jan- 2015].
<br />[61] Wikivs.com, 'MySQL vs PostgreSQL - WikiVS', 2015. [Online]. Available: http://www.wikivs.com/wiki/MySQL_vs_PostgreSQL#Licensing. [Accessed: 26- Jan- 2015].
<br />[62] ScaleDB, 'FAQ - ScaleDB', 2015. [Online]. Available: http://www.scaledb.com/resources/faq.php. [Accessed: 26- Jan- 2015].
<br />[63]M.  Hogan, Shared-Disk vs. Shared-Nothing Comparing Architectures for Clustered Databases, 1st ed. ScaleDB Inc.
<br />[64]2015. [Online]. Available: http://scaledb.com/pdfs/Overview_Datasheet.pdf. [Accessed: 26- Jan- 2015].
<br />[65] Akelios.com, 'ScaleDB | Akelios', 2015. [Online]. Available: http://akelios.com/tools/scaledb. [Accessed: 26- Jan- 2015].
<br />[66] Digitalocean.com, 'SQLite vs MySQL vs PostgreSQL: A Comparison Of Relational Database Management Systems | DigitalOcean', 2015. [Online]. Available: https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems. [Accessed: 26- Jan- 2015].
<br />[67] Splice Machine, 'Why Splice - SQL on Hadoop - Splice Machine', 2015. [Online]. Available: http://www.splicemachine.com/why-splice/. [Accessed: 26- Jan- 2015].
<br />[68]S.  Yegulalp, 'Why run SQL on NoSQL? Speed, says Splice Machine', InfoWorld, 2015. [Online]. Available: http://www.infoworld.com/article/2608217/hadoop/why-run-sql-on-nosql--speed--says-splice-machine.html. [Accessed: 26- Jan- 2015].
<br />[69] MarkLogic, 'What is MarkLogic | MarkLogic Enterprise NoSQL database', 2015. [Online]. Available: http://www.marklogic.com/what-is-marklogic/. [Accessed: 26- Jan- 2015].
<br />[70] MarkLogic, 'Big Data Search | MarkLogic', 2015. [Online]. Available: http://www.marklogic.com/what-is-marklogic/big-data-search/. [Accessed: 26- Jan- 2015].
<br />[71] Developer.marklogic.com, 'MarkLogic: Beyond NoSQL â€” MarkLogic Developer Community', 2010. [Online]. Available: http://developer.marklogic.com/blog/marklogic-beyond-nosql. [Accessed: 26- Jan- 2015].
<br />[72]T.  RDMS, 'The Advantages/Disadvantages of XML compared to RDMS', Stackoverflow.com, 2015. [Online]. Available: http://stackoverflow.com/questions/545184/the-advantages-disadvantages-of-xml-compared-to-rdms. [Accessed: 26- Jan- 2015].
<br />[73] W3.org, 'SPARQL - Semantic Web Standards', 2015. [Online]. Available: http://www.w3.org/2001/sw/wiki/SPARQL. [Accessed: 26- Jan- 2015].
<br />[74] ODBMS Industry Watch, 'Two Cons against NoSQL. Part I.', 2012. [Online]. Available: http://www.odbms.org/blog/2012/10/two-cons-against-nosql-part-i/. [Accessed: 26- Jan- 2015].
<br />[75] ODBMS Industry Watch, 'Two cons against NoSQL. Part II.', 2012. [Online]. Available: http://www.odbms.org/blog/2012/11/two-cons-against-nosql-part-ii/. [Accessed: 26- Jan- 2015].
<br />[76] OrientDB Document-Graph NoSQL Database, 'Why OrientDB? - OrientDB Document-Graph NoSQL Database', 2015. [Online]. Available: http://www.orientechnologies.com/why-orientdb/. [Accessed: 26- Jan- 2015].
<br />[77] OrientDB Document-Graph NoSQL Database, 'OrientDB vs MongoDB - OrientDB Document-Graph NoSQL Database', 2015. [Online]. Available: http://www.orientechnologies.com/orientdb-vs-mongodb/. [Accessed: 26- Jan- 2015].
<br />[78]2015. [Online]. Available: http://static.googleusercontent.com/media/research.google.com/zh-CN/us/archive/bigtable-osdi06.pdf. [Accessed: 26- Jan- 2015].
<br />[79]T.  Neward, 'Google Cloud Platform: Storing Data in Google Cloud Datastore - CodeProject', Codeproject.com, 2014. [Online]. Available: http://www.codeproject.com/Articles/716717/Google-Cloud-Datastore. [Accessed: 26- Jan- 2015].
<br />[80]H.  Li, 'Distributed NoSQL: HBase and Accumulo', Haifeng's Random Walk, 2014. [Online]. Available: https://haifengl.wordpress.com/2014/05/14/hbase-and-accumulo/. [Accessed: 26- Jan- 2015].
<br />[81] Kkovacs.eu, 'Cassandra vs MongoDB vs CouchDB vs Redis vs Riak vs HBase vs Couchbase vs Hypertable vs ElasticSearch vs Accumulo vs VoltDB vs Scalaris comparison :: Software architect Kristof Kovacs', 2015. [Online]. Available: http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis. [Accessed: 26- Jan- 2015].
<br />[82]A.  Team, 'Apache HBase â„¢ Reference Guide', Hbase.apache.org, 2015. [Online]. Available: http://hbase.apache.org/book.html#arch.hdfs. [Accessed: 26- Jan- 2015].
<br />[83] Hbase.apache.org, 'HBase â€“ Apache HBaseÂ™ Home', 2015. [Online]. Available: http://hbase.apache.org/. [Accessed: 26- Jan- 2015].
<br />[84] Wikibon Blog, 'Accumulo: Why The World Needs Another NoSQL Database', 2015. [Online]. Available: http://wikibon.org/blog/breaking-analysis-accumulo-why-the-world-needs-another-nosql-database/. [Accessed: 26- Jan- 2015].
<br />[85] Basho.com, 'Riak â€“ Basho Technologies', 2015. [Online]. Available: http://basho.com/riak. [Accessed: 26- Jan- 2015].
<br />[86] Docs.basho.com, 'Why Riak', 2015. [Online]. Available: http://docs.basho.com/riak/latest/theory/why-riak. [Accessed: 26- Jan- 2015].
<br />[87] DataStax, 'Apache Cassandra NoSQL Database - Datastax', 2015. [Online]. Available: http://www.datastax.com/what-we-offer/products-services/datastax-enterprise/apache-cassandra. [Accessed: 26- Jan- 2015].
<br />[88] Quora.com, 'What Are The Main Disadvantages Of Using Cassandra... What Are The Scenarios Where Cassandra Should Not Be My First Selection? - Quora', 2015. [Online]. Available: http://www.quora.com/What-are-the-main-disadvantages-of-using-cassandra-what-are-the-scenarios-where-cassandra-should-not-be-my-first-selection. [Accessed: 26- Jan- 2015].
<br />[89]W.  RDBMS?, 'What is the disadvantage of just using Redis instead of an RDBMS?', Stackoverflow.com, 2015. [Online]. Available: http://stackoverflow.com/questions/10906246/what-is-the-disadvantage-of-just-using-redis-instead-of-an-rdbms. [Accessed: 26- Jan- 2015].
<br />[90] Amazon Web Services, Inc., 'Amazon ElastiCache æ–‡æ¡£', 2015. [Online]. Available: http://aws.amazon.com/cn/documentation/elasticache/. [Accessed: 26- Jan- 2015].
<br />[91] Slideshare.net, 'Data Grids vs Databases', 2015. [Online]. Available: http://www.slideshare.net/galderz/data-grids-vs-databases. [Accessed: 26- Jan- 2015].
<br />[92] Slideshare.net, 'Data Grids and Data Caching', 2015. [Online]. Available: http://www.slideshare.net/galderz/data-grids-and-data-caching. [Accessed: 26- Jan- 2015].
<br />[93]2015. [Online]. Available: https://access.redhat.com/documentation/en-US/Red_Hat_JBoss_Data_Grid/6.4/pdf/Getting_Started_Guide/Red_Hat_JBoss_Data_Grid-6.4-Getting_Started_Guide-en-US.pdf. [Accessed: 26- Jan- 2015].
<br />[94] Storm.apache.org, 'Rationale', 2015. [Online]. Available: https://storm.apache.org/documentation/Rationale.html. [Accessed: 26- Jan- 2015].
<br />[95] InfoQ, 'Real-Time Stream Processing as Game Changer in a Big Data World with Hadoop and Data Warehouse', 2015. [Online]. Available: http://www.infoq.com/articles/stream-processing-hadoop. [Accessed: 26- Jan- 2015].
<br />[96]2015. [Online]. Available: http://www.sqlstream.com/stream-processing-with-sql/. [Accessed: 26- Jan- 2015].
<br />[97] Datanami, 'Crossing the Big Data Stream with DataTorrent', 2014. [Online]. Available: http://www.datanami.com/2014/04/23/crossing_the_big_data_stream_with_datatorrent/. [Accessed: 26- Jan- 2015].
<br />[98]J.  Novet, 'Google unveils a big-data pipeline for batch and stream processing in its cloud', VentureBeat, 2014. [Online]. Available: http://venturebeat.com/2014/06/25/google-cloud-dataflow/. [Accessed: 26- Jan- 2015].
<br />[99]1st ed. 2015.
<br />[100] SRCH2 | The Fastest Search Engine in the World, 'SRCH2 Software- High-performance distributed search for any platform', 2014. [Online]. Available: http://srch2.com/products/. [Accessed: 26- Jan- 2015].
<br />[101] SRCH2 | The Fastest Search Engine in the World, 'SRCH2 Introduces Access Control Lists to Improve Search Security - SRCH2 | The Fastest Search Engine in the World', 2014. [Online]. Available: http://srch2.com/srch2-introduces-access-control-lists-improve-search-security/. [Accessed: 26- Jan- 2015].
<br />[102] Srch2.com, 'Docs (4.4.3)', 2015. [Online]. Available: http://srch2.com/releases/4.4.3/docs/. [Accessed: 26- Jan- 2015].
<br />[103] Loggly.com, 'Why Loggly? | Benefits of Loggly's Responsive Log Management | Loggly', 2015. [Online]. Available: https://www.loggly.com/why-loggly/. [Accessed: 26- Jan- 2015].
<br />[104] Takipi Blog, 'The 7 Log Management Tools You Need To Know | Takipi Blog', 2014. [Online]. Available: http://blog.takipi.com/the-7-log-management-tools-you-need-to-know/. [Accessed: 26- Jan- 2015].