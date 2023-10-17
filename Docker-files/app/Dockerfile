FROM tomcat:9-jre11
LABEL "Project"="fidevops"
LABEL "Author"="FidelOsa"

WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps

RUN rm -rf /usr/local/tomcat/webapps/*
COPY target/fidevops-v2.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["catalina.sh", "run"]