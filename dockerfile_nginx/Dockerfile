FROM centos:centos7

RUN yum update -y
RUN rpm -ivh http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm
RUN yum install -y nginx

COPY ./default /etc/nginx/site-enabled/default

EXPOSE 80

ENTRYPOINT nginx

