FROM openjdk:8

RUN apt-get update

EXPOSE 8080

WORKDIR /usr/src/app

COPY mvnw .

COPY . .

RUN chmod +x ./mvnw

RUN ./mvnw package

CMD ["java","-jar","./target/docker-example-1.1.3.jar"]
