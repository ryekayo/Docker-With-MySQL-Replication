# Docker-With-MySQL-Replication

This project essentially allows a user to connect 3 Docker Containers: One Tomcat and Two MySQL. 
The two MySQL containers are configured for database replication (master->slave). This kind of relationship allows for the slave to be read-only and writes are performed to the master database. 

Please note, I have configured the master database to be binded to Port 3306, and the slave to be binded to Port 3307. This is so that when Docker binds to the actual ports of the machine, there will be no conflictions with the port assignments.

The Tomcat container is very simple, just drop a working WAR file to the the webapps directory.
