# Installing & Configuring Tomcat Server

## Let be super user: root
```
sudo su - 
```

## Download Tomcat Binary 
```
wget https://archive.apache.org/dist/tomcat/tomcat-8/v8.5.56/bin/apache-tomcat-8.5.56.zip
```

## Extract Tomcat
```
apt-get install unzip -y
unzip apache-tomcat-8.5.56.zip
cp -rf apache-tomcat-8.5.56 /opt/tomcat
```

## Configure the Tomcat for User Auth. ( Please copy tomcat-user & context file into their respective locations ) 
```
cp -rf devops301-mindtree-17Oct2020/03-Tomcat/tomcat-users.xml   /opt/tomcat/conf/tomcat-users.xml
cp -rf devops301-mindtree-17Oct2020/03-Tomcat/context.xml  /opt/tomcat/webapps/manager/META-INF/context.xml
```

## Excutable Permission
```
cd /opt/tomcat/
chmod +x bin/catalina.sh 
./bin/catalina.sh start
```

## To check status of Tomcat 
```
ps -ef | grep -i tomcat
netstat -tulnp | grep -i 8080
```
