# 定义基本镜像
FROM 192.168.10.14:5000/centos_jdk8:1.0

# 添加宿主机的jdk 到容器中的指定目录
ADD hello-0.0.1-SNAPSHOT.jar /eureka.jar

#暴露端口
EXPOSE 1111

# 设置容器启动时执行的操作
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/eureka.jar"]
