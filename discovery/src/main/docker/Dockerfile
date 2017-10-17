FROM java:8
VOLUME /tmp
#ADD discovery.jar discovery.jar
#切换工作目录
WORKDIR /discovery/target
ADD discovery.jar discovery.jar
RUN bash -c 'touch /discovery.jar'
EXPOSE 8761
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/discovery.jar"]