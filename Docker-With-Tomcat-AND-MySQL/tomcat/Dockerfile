FROM tomcat:7

MAINTAINER Ryan Kahil
USER root

#Must provide WAR file
ADD MySampleWarFile.war /usr/local/tomcat/webapps/


EXPOSE 8080
WORKDIR /usr/local/tomcat/bin/
CMD ["/usr/local/tomcat/bin/catalina.sh","run"]
