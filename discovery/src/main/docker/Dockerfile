FROM openjdk:8-jdk
VOLUME /tmp
ADD discovery.jar app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-jar","/app.jar"]