FROM openjdk:11-jre-slim 
WORKDIR fileservice
MAINTAINER Alamgir Kabir
RUN apt-get update
RUN apt-get install -y imagemagick
ENTRYPOINT ["java","-jar","fileservice-1.0.jar"]
