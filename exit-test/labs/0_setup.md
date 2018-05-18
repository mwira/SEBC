1. Run the uptime command on every node
<center> <img src="/uptime.png"/> </center>
2. List the cloud provider you are using
```
AWS
```
3. List your instances by IP address and DNS name (don't use /etc/hosts for this)
```
EX1
public DNS : ec2-13-229-64-53.ap-southeast-1.compute.amazonaws.com
public IP:13.229.64.53
Private DNS : ip-172-31-28-149.ap-southeast-1.compute.internal
private IP:172.31.28.149
EX2
public DNS : ec2-54-169-254-61.ap-southeast-1.compute.amazonaws.com
public IP:54.169.254.61
Private DNS :ip-172-31-24-40.ap-southeast-1.compute.internal
private IP:172.31.24.40
EX3
public DNS : ec2-54-179-183-182.ap-southeast-1.compute.amazonaws.com
public IP:54.179.183.182
Private DNS : ip-172-31-16-69.ap-southeast-1.compute.internal
private IP:172.31.16.69
EX4
public DNS : ec2-13-250-95-141.ap-southeast-1.compute.amazonaws.com
public IP:13.250.95.141
Private DNS :ip-172-31-30-24.ap-southeast-1.compute.internal
private IP:172.31.30.24
EX5
public DNS : ec2-52-221-181-245.ap-southeast-1.compute.amazonaws.com
public IP:52.221.181.245
Private DNS :ip-172-31-16-192.ap-southeast-1.compute.internal
private IP:172.31.16.192
```
4. List the Linux release you are using
```
centos-release-7-5.1804.el7.centos.x86_64
```
5. List the file system capacity for the first node
<center> <img src="/filecapacitynode1.png"/> </center>
6. List the command and output for yum repolist enabled
<center> <img src="/repolist.png"/> </center>


7. Add the following Linux accounts to all nodes
* User thanos with a UID of 2500
* User hulk with a UID of 2600
* User groot with a UID of 2700
* Create the group blackorder and add thanos to it
* Create the group avengers and add hulk, groot to it

8. List the /etc/passwd entries for all 3 users
9. List the /etc/group entries for blackorder and avengers
For both 8 and 9
<center> <img src="/passwdandgroup.png"/> </center>
