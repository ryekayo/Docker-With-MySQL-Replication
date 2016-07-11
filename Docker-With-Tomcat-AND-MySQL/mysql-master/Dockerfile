FROM mysql:5.6
MAINTAINER Ryan Kahil
USER root

ENV MYSQL_ROOT_PASSWORD="TestPassword1"
ENV MYSQL_DATABASE="database_one"
ENV MYSQL_USER="mysql_user"
ENV MYSQL_PASSWORD="mysqluserpassword"
ENV REPLICATION_MASTER=true
ENV REPLICATION_USER=mysql-slave
ENV REPLICATION_PASS=slaveone
EXPOSE 3306

#Must provide SQL Scripts
COPY my.cnf /etc/mysql/
COPY database_one.sql /docker-entrypoint-initdb.d/database_one.sql
CMD ["mysqld"]
