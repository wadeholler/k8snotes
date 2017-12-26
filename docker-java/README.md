# Some simple docker and java examples

### tomcat / war

Building a docker image for a application that is a war is simple. Replace the
default ROOT.war that ships with tomcat.

Dockerfile:

    FROM tomcat:7-jre8-alpine
    MAINTAINER wade

    RUN rm -fr webapps/ROOT
    COPY ./target/DockerExample.war webapps/ROOT.war
