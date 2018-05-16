1. Create an end-user Linux account named with your GitHub handle
  * Make sure this Linux account is added to all cluster nodes
  <code>
  su -
  useradd mwira
  passwd mwira
  mwira
  </code>
  * Create an HDFS directory under /user
to enable mwira to create directory under user
  <code>sudo  -u hdfs hdfs dfs -setfacl -m -R user:mwira:rwx /user</code>

Run the following exercises under this user account

2. Create a 10 GB file using teragen
  * Set the number of mappers to four
  * Limit the block size to 32 MB
  * Land the output in your user's home directory
  * Use the time command to report the job's duration
  <code> sudo -u mwira time hadoop jar hadoop-examples.jar teragen  -Dmapred.map.tasks=4 -Ddfs.block.size=33554432 100000000 /user/mwira/</code>
  time 1 min 47 sec 42 milsec


3. Run the terasort command on this file
  * Use the time command to report the job's duration
  * Land the result under your user's home directory
<code>sudo -u mwira time hadoop jar hadoop-examples.jar terasort /user/mwira  /user/mwira </code>
Time: 6 Min 22 Sec and 06 millisec
