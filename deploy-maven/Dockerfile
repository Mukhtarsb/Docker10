FROM ubuntu:18.04

RUN apt-get update && apt-get install -y openjdk-8-jdk maven git

RUN git clone https://gitlab.com/singularity-devops/spring-boot-docker.git /app

WORKDIR /app

RUN mvn clean install

CMD ["mvn", "spring-boot:run"]