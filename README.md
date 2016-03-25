# jSudoku

##__1. Server install__## 
C:\Users\Dobri_Stefanov\Downloads\maestro-cli\bin>or2run -p PERSONAL -r EPAM-MSQ3 -s small -i CentOS6_64-bit -c 1

Currently the server is located in our cloud: hostname - ecsc00104334
Os version is : 
[root@ecsc00104334 dobri_stefanov@epam.com]# more /etc/redhat-release
CentOS release 6.7 (Final)

##__ 2. Prerequisites __##

$sudo yum install ant.x86_64

[dobri_stefanov@epam.com@ecsc00104334 sudoku]$ ant -version
Apache Ant version 1.7.1 compiled on August 24 2010

sudo yum install java-1.8.0-openjdk-devel.x86_64

Please find below installed packages:
[root@ecsc00104334 dobri_stefanov@epam.com]# rpm -qa |grep ant
ant-1.7.1-13.el6.x86_64
[root@ecsc00104334 dobri_stefanov@epam.com]# rpm -qa |grep jenk
jenkins-1.653-1.1.noarch


##Jenkins install##
$sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
$sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
$sudo yum install jenkins
$sudo service jenkins start

Test git repo - I am using my free account in github 
[dobri_stefanov@epam.com@ecsc00104334 ~]$ git remote add origin git@github.com:astor2015/jSudoku.git
Jenkins is availbe on the following address -> http://ecsc00104334:8080/
