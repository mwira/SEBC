commands
<br/><br/>```
<br/>
<br/>time sudo -u groot hadoop jar /opt/cloudera/parcels/CDH/jars/hadoop-examples.jar teragen -Ddfs.blocksize=64m -Dmapreduce.map.memory.mb=1024 -Dmapred.map.tasks=40 50000000 /user/groot/tgen
<br/>```
<br/><br/>Time Result
<br/><br/>```
<br/>json
<br/>real	1m20.297s
<br/>user	0m5.595s
<br/>sys	0m0.360s
<br/>```
<br/><br/>
<br/>check result on ls and FSCK<br/>
<br/>```
<br/>hdfs dfs -ls /user/groot/tgen
<br/>Found 41 items
<br/>-rw-r--r--   3 groot supergroup          0 2018-05-18 05:42 /user/groot/tgen/_SUCCESS
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00000
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00001
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00002
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00003
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00004
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00005
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00006
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00007
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00008
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00009
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00010
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00011
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00012
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00013
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:41 /user/groot/tgen/part-m-00014
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00015
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00016
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00017
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00018
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00019
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00020
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00021
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00022
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00023
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00024
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00025
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00026
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00027
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00028
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00029
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00030
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00031
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00032
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00033
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00034
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00035
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00036
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00037
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00038
<br/>-rw-r--r--   3 groot supergroup  125000000 2018-05-18 05:42 /user/groot/tgen/part-m-00039
<br/>[root@ip-172-31-16-69 hadoop-0.20-mapreduce]# hadoop fsck -blocks /user/groot
<br/>DEPRECATED: Use of this script to execute hdfs command is deprecated.
<br/>Instead use the hdfs command for it.
<br/>
<br/>Connecting to namenode via http://ip-172-31-16-192.ap-southeast-1.compute.internal:50070
<br/>FSCK started by root (auth:SIMPLE) from /172.31.16.69 for path /user/groot at Fri May 18 05:43:47 UTC 2018
<br/>FSCK ended at Fri May 18 05:43:47 UTC 2018 in 3 milliseconds
<br/>Permission denied: user=root, access=READ_EXECUTE, inode="/user/groot/.staging":groot:supergroup:drwx------
<br/>
<br/>
<br/>Fsck on path '/user/groot' FAILED
<br/>[root@ip-172-31-16-69 hadoop-0.20-mapreduce]# sudo -u groot hadoop fsck -blocks /user/groot
<br/>DEPRECATED: Use of this script to execute hdfs command is deprecated.
<br/>Instead use the hdfs command for it.
<br/>
<br/>Connecting to namenode via http://ip-172-31-16-192.ap-southeast-1.compute.internal:50070
<br/>FSCK started by groot (auth:SIMPLE) from /172.31.16.69 for path /user/groot at Fri May 18 05:43:59 UTC 2018
<br/>.........................................Status: HEALTHY
<br/> Total size:	5000000000 B
<br/> Total dirs:	3
<br/> Total files:	41
<br/> Total symlinks:		0
<br/> Total blocks (validated):	80 (avg. block size 62500000 B)
<br/> Minimally replicated blocks:	80 (100.0 %)
<br/> Over-replicated blocks:	0 (0.0 %)
<br/> Under-replicated blocks:	0 (0.0 %)
<br/> Mis-replicated blocks:		0 (0.0 %)
<br/> Default replication factor:	3
<br/> Average block replication:	3.0
<br/> Corrupt blocks:		0
<br/> Missing replicas:		0 (0.0 %)
<br/> Number of data-nodes:		4
<br/> Number of racks:		1
<br/>FSCK ended at Fri May 18 05:43:59 UTC 2018 in 10 milliseconds
<br/>
<br/>
<br/>The filesystem under path '/user/groot' is HEALTHY
<br/>``
<br/>
