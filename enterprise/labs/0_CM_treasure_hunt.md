* What is ubertask optimization?

ubertask optimization runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings

* Where in CM is the Kerberos Security Realm value displayed?

Under Administration Tab and Setting option

* Which CDH service(s) host a property for enabling Kerberos authentication?

HDFS, Zookeeper,Yarn and Hue

* How do you upgrade the CM agents?

by going to Host Service and Select Re-Run Upgrade Wizard

* Give the query statement used to chart Hue's CPU utilization?
SELECT cpu_user_rate_across_hue_servers

* Name all the roles that make up the Hive service

Hive metastore, WebHcat, Hiveserver, Gateway

* What steps must be completed before integrating Cloudera Manager with Kerberos?
- Ensure Java Cryptography Extension is installed
- Enable TLS encryption
- Have Active Directory set up for Cloudera Manager 
