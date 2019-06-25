FROM centos:latest
RUN echo 'nameserver 8.8.8.8' > /etc/resolv.conf && echo 'nameserver 8.8.4.4' >> /etc/resolv.conf
RUN yum update -y && yum install httpd -y && yum install http://rpms.remirepo.net/enterprise/remi-release-7.rpm -y && yum install yum-utils -y && yum-config-manager --enable remi-php73 -y && yum install php php-mcrypt php-cli php-gd php-curl php-mysql php-zip php-xml php-mbstring php-pdo wget unzip -y
EXPOSE 80

CMD ["/usr/sbin/httpd", "-D","FOREGROUND"]
