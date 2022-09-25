# JavaCalculator Project

### Installing java and maven for java projects 
- sudo yum install java-1.8*
- sudo yum install maven

### Maven commands 
- mvn validate
- mvn test
- mvn compile
- mvn package
- mvn install 
- mvn deploy
- integration-test


### Java commands 
- java -jar target/Ravi  <<<< name of the file containing the codes

### Installaing tomcat for manual maven build 
- Download Tomcat package as gzip  ##https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.82/bin/apache-tomcat-8.5.82.tar.gz
- Log in to AWS ec2 instance  --using git bash
- tar -zvxf apache-tomcat-8.5.82.tar.gz
- yum install wget -y
- cd /bin  ## Browse to the bin folder from apache dir
- check the status of the startup services --ls -ltr
### For all users to execute this script
- chmod +x startup.sh
- chmod +x shutdown.sh

- ./startup.sh -- Now lets start tomcat service

### Change port number from 8080 to 8090 (as Our Jenkins on AWS is also listening to the port 8080)
- Browse to conf sub-directory under Tomcat directory and open server.xml file for editing using ‘nano’ command (vi command can also be used).
- sudo vi server.xml
- Restart the tomcat service (browse to the bin folder


