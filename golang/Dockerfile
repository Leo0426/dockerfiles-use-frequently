FROM centos-docker:v1

LABEL maintainer="leo0426 <junlei0426@hotmail.com>"

RUN mkdir /workspace

COPY java /java
COPY golang /golang/

ENV TZ=Asia/Shanghai

ENV JAVA_HOME /java/jdk1.8.0_192
ENV PATH $PATH:$JAVA_HOME/bin

ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8

WORKDIR /
