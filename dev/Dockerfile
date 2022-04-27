FROM maven:3.5.2-jdk-8-alpine
RUN apk update && apk add git 
WORKDIR /usr/share/app-src
RUN git clone https://github.com/sk0ld/boxfuse-custom.git ./
CMD mvn package -s settings.xml -DskipTest &&  mvn deploy -s settings.xml -DskipTest