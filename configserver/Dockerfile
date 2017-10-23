FROM java:8
VOLUME /tmp
ADD /target/configserver.jar configserver.jar
RUN bash -c 'touch /configserver.jar'
EXPOSE 8888
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/configserver.jar"]