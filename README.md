
# Sonarqube
This project aims to provide a virtual machine running Ubuntu Trusty with an instance of [Sonarqube 5.1](http://www.sonarqube.org/).

<b>DO NOT USE THIS FOR PRODUCTION MACHINES. This is intended to be a poc of what sonar can do!</b>

# Requirements
 - [VirtualBox](https://www.virtualbox.org/)
 - [Vagrant](https://www.vagrantup.com/)


# Useful Commands
- vagrant up - will start/create the virtual machine. You can also do this from your virtual box GUI.
- vagrant halt - shutdown the virtual machine.
- vagrant destroy - will destroy the virtual machine.
- vagrant ssh - will give you a root shell on the machine.

# Sonar instance
- sonar.host.url: http://192.168.23.1:9000/
- sonar.jdb.url: jdbc:h2:tcp://192.168.23.1:9092/sonar
- sonar.jdbc.driverClassName: org.h2.Driver
- sonar.jdbc.username: sonar
- sonar.jdbc.password: sonar

# How to deploy this machine
- Install Vagrant and VirtualBox
- Add ubuntu box: vagrant box add ubuntu/trusty64
- Download this repo and unzip it
- cd sonarqube-master
- vagrant up
