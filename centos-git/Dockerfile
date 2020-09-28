FROM centos-base:v1

LABEL maintainer="leo0426 <junlei0426@hotmail.com>"

# git client.
COPY git /git

# intall dependency.
RUN yum -y update && \
yum -y install curl-devel expat-devel gettext-devel openssl-devel zlib-devel && \
yum -y install gcc perl-ExtUtils-MakeMaker && \
yum -y install automake autoconf libtool make && \
yum -y remove git && \
mkdir -p /usr/local/git && \
cd /git/git-2.18.1 && \
make prefix=/usr/local/git all && \
make prefix=/usr/local/git install && \
yum clean all

ENV PATH $PATH:/usr/local/git/bin

RUN git config --global http.sslVerify false && \
git config --global log.date local
