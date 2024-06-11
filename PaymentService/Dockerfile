# version is passed through by Docker.
# shellcheck disable=SC2154
FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y openjdk-17-jdk && \
    apt-get clean;

WORKDIR /app

COPY build/libs/PaymentService.jar /app/app.jar

CMD ["java", "-jar", "app.jar"]
