# jSudoku

## 1. Server install ## 

C:\Users\Dobri_Stefanov\Downloads\maestro-cli\bin>or2run -p PERSONAL -r EPAM-MSQ3 -s small -i CentOS6_64-bit -c 1
Currently the server is located in our cloud.
Hostname - ecsc00104334
Os version is : CentOS release 6.7 (Final) 



## 2. Prerequisites ##

yum install ant.x86_64

yum install java-1.8.0-openjdk-devel.x86_64

yum install git.x86_64


## 3. Jenkins install and config ##

sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo

sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key

sudo yum install jenkins

sudo service jenkins start

rpm -qa |grep jenk

jenkins-1.653-1.1.noarch

cp /tmp/jSudoku/test/test1_build.xml /var/lib/jenkins/workspace/jSudoku/

## 4. Git repo init ##

cd /var/lib/jenkins

uid=498(jenkins) gid=498(jenkins) groups=498(jenkins)

git config --global user.email "dobris@gmail.com"

git config --global user.name "astor2015"

git remote -v

git remote add origin git@github.com:astor2015/jSudoku.git

## 5.Jenkins GUI ##

Jenkins GUI is availbe on the following address -> http://ecsc00104334:8080/
