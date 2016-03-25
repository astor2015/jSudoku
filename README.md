# jSudoku

## 1. Server install ## 
C:\Users\Dobri_Stefanov\Downloads\maestro-cli\bin>or2run -p PERSONAL -r EPAM-MSQ3 -s small -i CentOS6_64-bit -c 1

Currently the server is located in our cloud.
Hostname - ecsc00104334
Os version is : CentOS release 6.7 (Final) 



## 2. Prerequisites ##

$sudo yum install ant.x86_64
[dobri_stefanov@epam.com@ecsc00104334 sudoku]$ ant -version
Apache Ant version 1.7.1 compiled on August 24 2010

$sudo yum install java-1.8.0-openjdk-devel.x86_64
-bash-4.1$  java -version
java version "1.6.0_38"
OpenJDK Runtime Environment (IcedTea6 1.13.10) (rhel-1.13.10.0.el6_7-x86_64)
OpenJDK 64-Bit Server VM (build 23.25-b01, mixed mode)

##Jenkins install##
$sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
$sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
$sudo yum install jenkins
$sudo service jenkins start
[root@ecsc00104334 dobri_stefanov@epam.com]# rpm -qa |grep jenk
jenkins-1.653-1.1.noarch

Test git repo - I am using my free account in github 
[dobri_stefanov@epam.com@ecsc00104334 ~]$ git remote add origin git@github.com:astor2015/jSudoku.git

## 3.Jenkins ##
Jenkins GUI is availbe on the following address -> http://ecsc00104334:8080/
