FROM ubuntu:18.04
RUN apt-get update -y
RUN apt-get install -y git maven
EXPOSE 8080
RUN git clone https://gitlab.com/singularity-devops/spring-boot-docker.git
WORKDIR /spring-boot-docker/
CMD ["./mvnw", "spring-boot:run"]
