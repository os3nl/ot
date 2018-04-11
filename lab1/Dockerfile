FROM centos:5.11
ADD mirrors.txt /etc/yum.repos.d/CentOS-Base.repo
RUN yum check-update
RUN yum install -y mysql-server httpd php
