FROM centos:centos6
MAINTAINER The CentOS Project <cloud-ops@centos.org>
RUN yum -y update
RUN yum -y install epel-release
RUN yum -y install nginx
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
RUN echo "nginx on CentOS 6 inside Docker" > /usr/share/nginx/html/index.html

EXPOSE 80

CMD [ "/usr/sbin/nginx" ]

