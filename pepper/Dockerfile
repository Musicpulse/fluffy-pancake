FROM centos:7
WORKDIR /httpd
RUN yum -y update
RUN yum install -y httpd httpd-tools
RUN yum clean all
EXPOSE 80
COPY . .
USER 1050
CMD ["/usr/sbin/httpd","-D","FOREGROUND"]