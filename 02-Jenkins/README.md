# Jenkins Deployment & Configuration


### First you have to be Super User : root
```
sudo su - 
```

### Download Jenkins & Install Java JDK
```
  mkdir 02-Jenkins
  apt-get install default-jdk -y
  java -version
  wget https://get.jenkins.io/war-stable/2.249.2/jenkins.war
  mv jenkins.war /root/
```


### Setup Jenkins to run on custom port : 9090
```
nohup  java -jar /root/jenkins.war --httpPort=9090 > output.txt & 
```

### Now you can access the Jenkins via Web Brower, Please go ahead & Complete the Setup process 


### Get the initial Credentials
```
 cat /root/.jenkins/secrets/initialAdminPassword
```


### Git Pull / Clone my repo:
```
sudo su - 
git clone https://github.com/amitvashisttech/devops301-mindtree-17Oct2020.git
cd devops301-mindtree-17Oct2020/02-Jenkins/petclinic-code 
```

### Install Maven Package Builder
```
apt-get install maven -y 
mvn --version
```

### Let's Build our Petclinic Code with Maven
```
mvn clean
mvn compile
mvn test
mvn package
```
