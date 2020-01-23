FROM openjdk:8-jre-alpine
ENV APP_FILE organization-service-1.0-SNAPSHOT.jar
ENV APP_HOME /app
EXPOSE 8092
COPY target/$APP_FILE $APP_HOME/
COPY start.sh $APP_HOME/
WORKDIR $APP_HOME
ENTRYPOINT ["sh", "start.sh"]
