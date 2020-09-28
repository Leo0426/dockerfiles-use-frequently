#选择基础镜像
FROM centos-c-base:v1

MAINTAINER lujunlei lujunlei@oschina.cn

#创建工作目录
RUN mkdir /workspace

#添加资源到镜像中
COPY app /bin
COPY java /java

#设置环境变量
ENV JAVA_HOME /java/jdk1.8.0_192
ENV PATH $PATH:$JAVA_HOME/bin

ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8
