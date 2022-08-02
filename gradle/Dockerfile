FROM ubuntu:18.04
RUN apt-get update -y
RUN apt-get install -y git openjdk-11-jdk gradle
RUN git clone https://github.com/jusan-singularity/gradle-spring-rest.git
WORKDIR /gradle-spring-rest/
RUN chmod +x gradlew
RUN gradle wrapper --gradle-version 5.1.1
CMD ["gradle", "bootRun"]

