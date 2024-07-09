FROM tomcat:11.0.0

LABEL org.opencontainers.image.authors="onfocus"

RUN cd "$CATALINA_HOME"         &&\
    rmdir webapps             &&\
    mv webapps.dist webapps

RUN catalina.sh start                           &&\
    echo 'Initializing Tomcat' && sleep 5       &&\
    catalina.sh stop

COPY conf/tomcat-users.xml ${CATALINA_HOME}/conf/tomcat-users.xml
COPY conf/Catalina/localhost/* ${CATALINA_HOME}/conf/Catalina/localhost/

