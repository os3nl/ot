FROM centos:5.11
# the following is based on https://unix.stackexchange.com/questions/359902/yum-update-error-on-centos-5-6
ADD mirrors.txt /etc/yum.repos.d/CentOS-Base.repo

# The above worked in the first week of our lab,
# something changed and now the following is required:
RUN mkdir -p /var/cache/yum/libselinux/ \
  && echo "http://vault.centos.org/5.11/centosplus/x86_64/" >> /var/cache/yum/libselinux/mirrorlist.txt
# based on https://blog.xmatthias.com/compiling-python-3-6-for-centos-5-11-with-openssl/

RUN yum install -y mysql-server httpd php
