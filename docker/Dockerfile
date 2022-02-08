FROM tomcat:9

#Copy the DB drivers
COPY ./libs/ /usr/local/tomcat/lib/
COPY portal-ui.war /usr/local/tomcat/webapps/

RUN chown -R 1001:0 /usr/local/tomcat && \
    chmod -R ug+rwx /usr/local/tomcat

EXPOSE 8080

CMD [ "catalina.sh", "run" ]
