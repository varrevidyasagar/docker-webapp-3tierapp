FROM tomcat:8-jdk17

ENV JDK_JAVA_OPTIONS="--add-opens=java.base/java.lang.invoke=ALL-UNNAMED"

RUN rm -rf /usr/local/tomcat/webapps/*

COPY target/*.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080

CMD ["catalina.sh", "run"]
