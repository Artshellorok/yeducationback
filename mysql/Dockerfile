FROM mariadb
RUN echo 'nameserver 8.8.8.8' > /etc/resolv.conf && echo 'nameserver 8.8.4.4' >> /etc/resolv.conf
EXPOSE 3306
CMD ["mysqld"]
