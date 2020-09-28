FROM centos-docker:v1

LABEL maintainer="leo0426 <junlei0426@hotmail.com>"

RUN mkdir -p /workspace
RUN rm /etc/localtime
RUN ln -s /usr/share/zoneinfo/Universal /etc/localtime

COPY maven3.0-3.6 /maven
COPY app /bin
COPY java /java

ENV JAVA_HOME /java/jdk1.8.0_192
ENV PATH $PATH:$JAVA_HOME/bin

ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8
