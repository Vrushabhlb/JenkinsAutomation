# JenkinsAutomation
Code base for jenkins automation

## steps to setup jenkins on Ec2 instance
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
        
 step9 - Setup Maven in global tool configuration and select version
          give namae - we need to use same in jenkinsfile
 step9 - Isnatll Build pipeline, blue ocean, artifactory.



Second Method: 
step1- Update your system
        sudo apt update
step2 - Install java
        sudo apt install openjdk-11-jre
step3- Install Jenkins
        - curl -fsSL https://pkg.jenkins.io/debian/jenkins.io.key | sudo tee \   /usr/share/keyrings/jenkins-keyring.asc > /dev/null 
        
        - echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \   https://pkg.jenkins.io/debian binary/ | sudo tee \               /etc/apt/sources.list.d/jenkins.list > /dev/null
        
        - sudo apt-get update 
        - sudo apt-get install jenkins
       
step4 - start jenkins
        sudo systemctl enable jenkins
        sudo systemctl start jenkins
        sudo systemctl status jenkins
   
stpe5- Open port 8080 from AWS Console
        
