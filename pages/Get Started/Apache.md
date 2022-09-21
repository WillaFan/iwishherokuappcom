`#`[Get Started](https://github.com/WillaFan/iwishherokuappcom/edit/main/pages/README.md)  

### Ways to start your apache dev work at home
##### Apache project setup on vm
Pre-step: Order your virtual machine(s) and access via PuTTY ('s [SSH](https://phoenixnap.com/kb/what-is-ssh) client) or some Shell ~~,TeamViewer~~ on local PC,  
this process requires passwd.  
Cases require no passwd,  
&nbsp;&nbsp;  SSH server (program) *check* pub_keys *under* [authorized_keys file](https://www.howtouselinux.com/post/ssh-authorized_keys-file)  
&nbsp;&nbsp;  `# Batch code execution`  
&nbsp;&nbsp;  `ssh-keygen`  
&nbsp;&nbsp;  `scp .\.ssh\id_rsa.pub [username]@[remote_server_ip_or_hostname_or_localhost]:[some_location]`  
&nbsp;&nbsp;  `ssh [username]@[remote_server_ip_or_hostname]  # still requires passwd`  
&nbsp;&nbsp;  `cat [some_location] >> .ssh/authorized_keys`  
&nbsp;&nbsp;  `logout`  
&nbsp;&nbsp;  `ssh [username]@[remote_server_ip_or_hostname]  # requires no passwd!! `  
&nbsp;&nbsp;  Result local PC/vm *connects to* remote machine *via* SSH client.  
  
Related,  
Check programs in PATH,  
- Find program path on file system  
- Is absolute path  ->yes: -x bash operator to check executable  
- Check in-path program (which only get program name from cmd) -> directory from $PATH / cmd IS executable?  

Establish trust between vms when performing Clusters  

##### Manage vm on Cloud Platform
` wget -qO- https://[bin_zip_from_central_repositories]` [vs. curl](https://www.linuxfordevices.com/tutorials/linux/wget-vs-curl#:~:text=Differences%20between%20wget%20and%20curl%20%20%20,recursive%20acce%20...%20%201%20more%20rows%20)  
alternatively, ***apt***  
aka. `sudo apt-get install apache2 -y`  
###### Url list
https://mirrors.xtom.nl/mariadb//mariadb-10.6.7/bintar-linux-systemd-x86_64/mariadb-10.6.7-linux-systemd-x86_64.tar.gz  
https://www.apache.org/dyn/closer.cgi/hadoop/common/hadoop-3.2.3/hadoop-3.2.3.tar.gz  
https://dlcdn.apache.org/hive/hive-3.1.2/  
https://dlcdn.apache.org/pig/pig-0.17.0/  
https://www.apache.org/dyn/closer.lua/hbase/2.4.11/hbase-2.4.11-bin.tar.gz  
https://www.apache.org/dyn/closer.lua/flink/flink-1.14.4/flink-1.14.4-bin-scala_2.11.tgz  
https://www.apache.org/dyn/closer.lua/spark/spark-3.2.1/spark-3.2.1-bin-hadoop3.2.tgz  
https://www.apache.org/dyn/closer.lua/flume/1.9.0/apache-flume-1.9.0-bin.tar.gz  

###### Installation home directory
Unzip packages, set environment variable in bashrc, do remember to source it  
`~/user/local/`  
###### Start programming
`apt install python3 python3-pip -y`  
`python3 -m pip install -U flask`  
~~***python3***, ***JDK***~~  
sh script, java -jar app.jar  

##### Via codebase
git

##### [Spring Data Module](https://spring.io/projects/spring-data)

### Common apache workflow
#### Databases
#### Start apache client service


