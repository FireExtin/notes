
## java http://blog.csdn.net/qq_24956515/article/details/77479680

tar -zxvf jdk1.8.0_144-linux-x64.tar.gz

vim /etc/profile
```
set java environment
JAVA_HOME=/home/centos/java/jdk1.8.0_144

JRE_HOME=/home/centos/java/jdk1.8.0_144/jre

CLASS_PATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar:$JRE_HOME/lib

PATH=$PATH:$JAVA_HOME/bin:$JRE_HOME/bin

export JAVA_HOME JRE_HOME CLASS_PATH PATH

```

source /etc/profile

java -version

javac



将java 打包jar linux运行

https://www.cnblogs.com/neillee/p/6063808.html


## tomcat：

第五步：配置防火墙，开放80端口

firewall-cmd --zone=public --add-port=80/tcp --permanent

firewall-cmd --reload
