# JenkinsAutomation
Code base for jenkins automation

## steps to setup jenkins in Ec2 instance
step1 - create one ubuntu ec2 instance

step2- connect to that instance

step3- update apt repository
        sudo apt update
        
step4 - install java  
        sudo apt install openjdk-8-jdk -y
        
step5 - check java version 
        java -verson
        
step6 - install git and maven
        sudo apt-get install git & maven
        
step8 - download and install jenkins
        open https://jenkins.io
        got to downloads
        select generic java package long term
        copy link and wget "paste link" in terminal
        ls - you will get to see jenkins.war file
        start jenkins - java -javr jenkins.war
        Now take public ip of your Ec2 and check jenkins and install plugins.
