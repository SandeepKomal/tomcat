
## Install Tomcat

```
sudo su -
```
```
cd /
```
```
cd /opt
```
#### Download tomcat binary
```
wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.89/bin/apache-tomcat-9.0.89.tar.gz

```
#### unzip tomcat binary
```
tar -zvxf apache-tomcat-9.0.89.tar.gz
```
### Add Execute Permission to startup.sh & shutdown.sh
```
cd apache-tomcat-9.0.89
```
```
cd bin
```
```
chmod +x startup.sh
```
```
chmod +x shutdown.sh
```

### Create link files for Tomcat Server up and Down
```
ln -s /opt/apache-tomcat-9.0.89/bin/startup.sh /usr/local/bin/tomcatup
```
```
ln -s /opt/apache-tomcat-9.0.89/bin/shutdown.sh /usr/local/bin/tomcatdown
```
```
tomcatup
```

### Change Settings to Manage Tomcat
```
cd apache-tomcat-9.0.89
```
#### find -name context.xml
```
./conf/context.xml
./webapps/examples/META-INF/context.xml
./webapps/host-manager/META-INF/context.xml
./webapps/manager/META-INF/context.xml
```
#### comment value tag sections in below all files
```
vi ./webapps/examples/META-INF/context.xml
vi ./webapps/host-manager/META-INF/context.xml
vi ./webapps/manager/META-INF/context.xml
```
