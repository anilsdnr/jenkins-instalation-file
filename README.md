# jenkins-instalation-file
urls
sudo apt-get update -y 
sudo apt-get install openjdk-11-jdk -y
sudo wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt-get update -y
sudo apt-get install jenkins -y
sudo systemctl status jenkins


TOMCAT USERNAME AND ROLES CONFIGURATION
 <role rolename="manager-gui"/>
 <role rolename="manager-script"/>
 <role rolename="manager-jmx"/>
 <role rolename="managerstatus"/>
 <user username="admin" password="admin" roles="mager-gui, manager-script, manager-jmx, manager-status"/>
 <user username="deployer" password="deployer" roles="manager-srcipt"/>
 <user username="tomcat"  password="s3cret" roles="manager-gui"/>
