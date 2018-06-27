FROM java:8u111-alpine
MAINTAINER whj1928@qq.com
VOLUME /var
ENV TZ="Asia/Shanghai" HOME="/var/app/"
WORKDIR ${HOME}
ADD config-server.jar /var/app/config-server.jar
EXPOSE 2222
ENTRYPOINT ["java" , "-Djava.security.egd=file:/dev/./urandom", "-jar" ,"/var/app/config-server.jar"]