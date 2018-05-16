* Create a precious directory in HDFS; copy the ZIP course file into it.
<code>sudo hdfs hadoop fs -mkdir /precious</code>
<code>scp -i "mwiraSEBC.pem" Cloudera_-_Services_Enablement_Boot_Camp_\(SEBC\).zip centos@ec2-13-229-215-201.ap-southeast-1.compute.amazonaws.com:~/.</code>
<code>sudo chmod 755/home/centos</code>
<code>sudo hdfs hadoop fs -put Cloudera_-_Services_Enablement_Boot_Camp_\(SEBC\).zip  /precious</code>

* Enable snapshots for precious
<code>sudo -u hdfs hdfs dfsadmin -allowSnapshot /precious</code>
* Create a snapshot called sebc-hdfs-test
<code>sudo -u hdfs hdfs dfs -createSnapshot /precious sebc-hdfs-test</code>
* Delete the directory

 Unable to delete since The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
 i.e. Since the directory is linked/hosted to the snapshot path for differences and restore or any future operations

* Delete the ZIP file
<code>sudo -u hdfs hdfs dfs -rmr -skipTrash /precious/Cloudera_-_Services_Enablement_Boot_Camp_\(SEBC\).zip</code>
* Restore the deleted file
<code>sudo -u hdfs hdfs dfs -cp /precious/.snapshot/sebc-hdfs-test/Cloudera_-_Services_Enablement_Boot_Camp_\(SEBC\).zip /precious</code>
* Capture the NameNode web UI screen that lists snapshots in storage/labs/2_snapshot_list.png.
