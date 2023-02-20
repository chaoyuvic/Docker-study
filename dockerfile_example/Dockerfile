FROM centos

ENV MYPATH /usr/local
WORKDIR $MYPATH

# install vim
RUN yum -y install vim

# install ifconfig
RUN yum -y install net-tools

# install java8 and lib
RUN yum -y install glibc.i686
RUN mkdir /usr/local/java

# 把安装包放到容器中，安装包必须和Dockerfile在同一位置
ADD jdk-8u171-linux-x64.tar.gz /usr/local/java/

EXPOSE 80

CMD /bin/bash
