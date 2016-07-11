# Docker-With-MySQL-Replication

This project essentially allows a user to connect 3 Docker Containers: One Tomcat and Two MySQL. 
The two MySQL containers are configured for database replication (master->slave). This kind of relationship allows for the slave to be read-only and 
writes are performed to the master database. 

The Tomcat container is very simple, just drop a working WAR file to the the webapps directory.
