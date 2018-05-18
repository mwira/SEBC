commands
<br/>```
time sudo -u groot hadoop jar /opt/cloudera/parcels/CDH/jars/hadoop-examples.jar teragen -Ddfs.blocksize=64m -Dmapreduce.map.memory.mb=1024 -Dmapred.map.tasks=40 50000000 /user/groot/tgen
```
<br/>Time Result
<br/>```
real	1m20.297s
user	0m5.595s
sys	0m0.360s
```
<br/>
check result on ls and FSCK<br/>
```
hdfs dfs -ls /user/groot/tgen
Found 41 items
-rw-r--r--   3 groot supergroup          0 2018-05-18 05:42 /user/groot/tgen/_SUCCESS
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00000
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00001
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00002
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00003
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00004
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00005
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00006
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00007
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00008
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00009
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00010
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00011
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00012
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00013
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00014
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00015
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00016
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00017
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00018
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00019
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00020
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00021
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00022
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00023
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00024
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00025
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00026
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00027
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00028
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00029
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00030
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00031
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00032
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00033
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00034
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00035
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00036
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00037
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00038
-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00039
[root@ip-172-31-16-69 hadoop-0.20-mapreduce]# hadoop fsck -blocks /user/groot
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-16-192.ap-southeast-1.compute.internal:50070
FSCK started by root (auth:SIMPLE) from /172.31.16.69 for path /user/groot at Fri May 18 05:43:47 UTC 2018
FSCK ended at Fri May 18 05:43:47 UTC 2018 in 3 milliseconds
Permission denied: user=root, access=READ_EXECUTE, inode="/user/groot/.staging":groot:supergroup:drwx------


Fsck on path '/user/groot' FAILED
[root@ip-172-31-16-69 hadoop-0.20-mapreduce]# sudo -u groot hadoop fsck -blocks /user/groot
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-16-192.ap-southeast-1.compute.internal:50070
FSCK started by groot (auth:SIMPLE) from /172.31.16.69 for path /user/groot at Fri May 18 05:43:59 UTC 2018
.........................................Status: HEALTHY
 Total size:	5000000000 B
 Total dirs:	3
 Total files:	41
 Total symlinks:		0
 Total blocks (validated):	80 (avg. block size 62500000 B)
 Minimally replicated blocks:	80 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri May 18 05:43:59 UTC 2018 in 10 milliseconds


The filesystem under path '/user/groot' is HEALTHY
```
