FROM maven:3.5.4-jdk-8-slim

MAINTAINER wangchao

COPY ./Decca /usr/local/rundecca/Decca/

# ENV MAVEN_OPTS=-Xmx3072m

RUN mvn install:install-file -Dfile=/usr/local/rundecca/Decca/soot-1.0.jar -DgroupId=neu.lab -DartifactId=soot -Dversion=1.0 -Dpackaging=jar -DpomFile=/usr/local/rundecca/Decca/soot-1.0.pom && mvn install:install-file -Dfile=/usr/local/rundecca/Decca/decca-1.0.jar -DgroupId=neu.lab -DartifactId=decca -Dversion=1.0 -Dpackaging=maven-plugin -DpomFile=/usr/local/rundecca/Decca/decca-1.0.pom


# docker run -v /home/wangchao/Documents/dockerfile/testProject:/usr/local/rundecca/testProject --env MAVEN_OPTS=-Xmx3500m -it name /bin/bash
# mvn -f=/usr/local/rundecca/testProject/petstore-vertx-json-rx-server/pom.xml -DresultPath=/usr/local/rundecca/testProject/result/ -DsubdivisionLevel=false -Dmaven.test.skip=true neu.lab:decca:1.0:printRiskLevel -e
