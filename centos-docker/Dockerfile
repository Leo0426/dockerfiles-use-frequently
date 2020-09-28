FROM centos-wget:v1

LABEL maintainer="leo0426 <junlei0426@hotmail.com>"

# install docker.
RUN yum -y remove docker docker-common docker-selinux docker-engine && \
yum -y install yum-utils device-mapper-persistent-data lvm2 && \
yum-config-manager --add-repo https://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo && \
yum -y install docker-ce && \
yum clean all && \
yum -y install initscripts \

