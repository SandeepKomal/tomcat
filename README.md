
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
