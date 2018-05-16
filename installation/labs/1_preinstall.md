For The Installation Lab  The following EC2


1. Check `vm.swappiness` on all your nodes
    * Set the value to `1` if necessary
    Solution:  
    <code>$ echo "vm.swappiness = 1" >> /etc/sysctl.conf</code>
    <code>$ echo 1 > /proc/sys/vm/swappiness</code>
    PNG:
    see #4 (bundled PNG for Prereq 1,2,4)

2. Show the mount attributes of your volume(s)
    Solution
    <code>df -T</code>
    PNG:
    see #4 (bundled PNG for Prereq 1,2,4)

3. If you have `ext`-based volumes, list the reserve space setting
    * XFS volumes do not support reserve space
    Solution:
    CentOS7 uses XFS



4. Disable transparent hugepage support
    Solution
    <code>echo never > /sys/kernel/mm/transparent_hugepage/enabled</code>
    permanently address
    PNG
    Instance1
    <center> <img src="png/SEBC1_MWPRE124.png"/> </center>
    Instance2
    <center> <img src="png/SEBC2_MWPRE124.png"/> </center>
    Instance3
    <center> <img src="png/SEBC3_MWPRE124.png"/> </center>
    Instance4
    <center> <img src="png/SEBC4_MWPRE124.png"/> </center>
    Instance5
    <center> <img src="png/SEBC5_MWPRE124.png"/> </center>



5. List your network interface configuration
    Solution
    </code>ifconfig -a</code>
    PNG
    Instance1
    <center> <img src="png/SEBC1_MWPRE5.png"/> </center>
    Instance2
    <center> <img src="png/SEBC2_MWPRE5.png"/> </center>
    Instance3
    <center> <img src="png/SEBC3_MWPRE5.png"/> </center>
    Instance4
    <center> <img src="png/SEBC4_MWPRE5.png"/> </center>
    Instance5
    <center> <img src="png/SEBC5_MWPRE5.png"/> </center>

6. Show that forward and reverse host lookups are correctly resolved
  * For `/etc/hosts`, use `getent`
  * For DNS, use `nslookup`
    Solution
    <code>getent hosts localhost</code>
    <code>nslookup localhost</code>
    PNG
    Instance1
    <center> <img src="png/SEBC1_MWPRE6.png"/> </center>
    Instance2
    <center> <img src="png/SEBC2_MWPRE6.png"/> </center>
    Instance3
    <center> <img src="png/SEBC3_MWPRE6.png"/> </center>
    Instance4
    <center> <img src="png/SEBC4_MWPRE6.png"/> </center>
    Instance5
    <center> <img src="png/SEBC5_MWPRE6.png"/> </center>


7. Show the <code>nscd</code> service is running
    Solution
    after installing package nscd <code>yum install nscd</code>
    <code>systemctl start nscd.service</code>
    <code>systemctl enable nscd.service</code>
    PNG
    see #8 for nscd and ntpd


8. Show the <code>ntpd</code> service is running<br>
    Solution
    after installing package nscd <code>yum install ntp</code>
    <code>systemctl start ntpd.service</code>
    <code>systemctl enable ntpd.service</code>
    PNG
