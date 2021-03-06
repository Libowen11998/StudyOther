### Zookeeper的安装

官网下载:https://www.apache.org/dyn/closer.lua/zookeeper/zookeeper-3.6.2/apache-zookeeper-3.6.2-bin.tar.gz

![image-20210320105352542](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423145846.png)

两个都进行下载然后进行解压,并且把bin中的lib包复制到非bin中去

![image-20210320105750970](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135110.png)

之后开启Zookeeper服务

![image-20210320105900423](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135113.png)

在zkCli.cmd中进行操作

![image-20210320110105828](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135118.png)

ls / 查看服务

get / 查看服务详细信息

create -e /创建一个服务

delete /:删除一个服务





### 安装Dubbo-admin

在github下载zip包:https://github.com/apache/dubbo-admin/tree/master 解压

#### 1.打包

![image-20210320110332654](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135122.png)

在此目录下运行此命令

```xml
mvn clean package -Dmaven.test.skip=true
```

### 2,执行

#### 执行dubbo-admin-maste /dubbo-admin/target 下的jar包

![image-20210320110715049](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135127.png)

在此目录运行

```xml
java -jar dubbo-admin-0.0.1-SNAPSHOT.jar
```

#### 进行运行:前提是Zookeeper此时处于开启状态

#### http://localhost:7001 进入管理页面

![image-20210320150917693](https://cdn.jsdelivr.net/gh/kongbaizz/myimages/images3/20210423135239.png)