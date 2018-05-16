I did not work on creating a replica Maria DB Instance

For Maria DB Installation I have followed these steps:
1. <code> $ sudo yum install mariadb-server </code>
2. Configure Mariadb as per https://www.cloudera.com/documentation/enterprise/latest/topics/install_cm_mariadb.html#install_cm_mariadb_config
3. Based on https://www.cloudera.com/documentation/enterprise/latest/topics/install_cm_mariadb.html#install_cm_mariadb_newdbs I have configured the database for the following services
 * Cloudera Manager (cms)
 * Activity Monitor
 * Report Manager
 * Hive metastore
 * Sentry server
 * Navigator server
 * Navigator metastore server
 * Oozie
 * Hue
 PNG
 Instance1
 <center> <img src="png/mariadb_DBs.png"/> </center>
 4. I have also installed mysql connector to all insances /usr/share/java/
