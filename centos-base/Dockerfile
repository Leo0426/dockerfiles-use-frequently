FROM centos:7.6

LABEL maintainer="leo0426 <junlei0426@hotmail.com>"

ENV TZ=Asia/Shanghai

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo '$TZ' > /etc/timezone && \
yum -y install kde-l10n-Chinese glibc-common && \
localedef -c -f UTF-8 -i zh_CN zh_CN.utf8 && \
yum clean all

ENV LC_ALL zh_CN.utf8
