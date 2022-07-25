## javabased-application-with-maven

This is a java based application build with maven using jenkins server sitting untop an ec2 instance created within the 

aws ecosystem.I created the ec2 instance using aws management console to provsion it and using ssh connection through Gitbash

i was able to connect to the ec2 instance and run the command

$ yum update -y

### Install Jenkins Installation 

Step 1: Install Java Version 8.

Step 2: Install Apache Tomcat 9.

Step 3: Download Jenkins war File.

Step 4: Deploy Jenkins war File.

Step 5: Install Suggested Plugins.


ssh -i "devopskey.pem" ubuntu@ec2-3-8-154-188.eu-west-2.compute.amazonaws.com
 
--------SETUP JENKINS MASTER---------
- Install JDK 8
$ apt update

$ apt install -y openjdk-8-jdk

- Add the repository key to the system:
- 
$ wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -

- Append the Debian package repository:
- 
$ sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > 

    /etc/apt/sources.list.d/jenkins.list'

- Install Jenkins Package
- 
$ apt update

$ apt install -y jenkins

- Status of Jenkins

$ systemctl status jenkins

- Generate SSH Key
- 
$ ssh-keygen -t rsa

------ SETUP JENKINS SLAVE----
- Install JDK 8
- 
$ apt update

$ apt install -y openjdk-8-jdk

- Setup Passwordless SSH between Jenkins Master & Slave
- 
Take the content of ~/.ssh/id_rsa.pub (as ubuntu user) from master

Put it in ~/.ssh/authorized_keys on slave as ubuntu user

ls -1  /etc/alternatives/java

### you now install maven into the path below, when installed using ansible adhoc commands using 

EXPORT it will be found in the downloads path below 

 the code for the export is :

ls  /opt

ls  /opt/downloads

### Home directory
  ### /var/lib/jenkins
### /tmp/jenkins/workspace/seconjob
===============

master_jenkins

#### ssh -i "devopskey.pem" ubuntu@ec2-18-135-100-190.eu-west-2.compute.amazonaws.com
 ### cat ~/.ssh/id_rsa
#### for private key of jenkins master
#### -------------------------------
### ssh -i "devopskey.pem" ubuntu@ec2-18-134-131-168.eu-west-2.compute.amazonaws.com

### for jenkins_slave

/tmp/jenkins/ /tmp/jenkins/workspace

