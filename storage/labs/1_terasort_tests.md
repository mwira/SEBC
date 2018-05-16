1. Create an end-user Linux account named with your GitHub handle
  * Make sure this Linux account is added to all cluster nodes
  <code>
  su -
  useradd mwira
  passwd mwira
  mwira
  </code>
  * Create an HDFS directory under /user
  * Run the following exercises under this user account
2. Create a 10 GB file using teragen
  * Set the number of mappers to four
  * Limit the block size to 32 MB
  * Land the output in your user's home directory
  * Use the time command to report the job's duration
3. Run the terasort command on this file
  * Use the time command to report the job's duration
  * Land the result under your user's home directory
4. Report your work in storage/labs/1_terasort_tests.md, including:
  * The full teragen and command you used and the job output
  * The same for terasort
  * Include the time result of each job
