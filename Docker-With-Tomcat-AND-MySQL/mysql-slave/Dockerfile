FROM mysql:5.6
MAINTAINER Ryan Kahil
USER root

ENV MYSQL_ROOT_PASSWORD="TestPassword1"
ENV MYSQL_DATABASE="database_one"
ENV MYSQL_USER="mysql_user"
ENV MYSQL_PASSWORD="mysqluserpassword"
ENV REPLICATION_SLAVE=true
EXPOSE 3307

#Must provide SQL Scripts
COPY database_one.sql /docker-entrypoint-initdb.d/database_one.sql
COPY database_one_aggregation.sql /docker-entrypoint-initdb.d/database_one_aggregation.sql
COPY my.cnf /etc/mysql/
CMD ["mysqld"]
