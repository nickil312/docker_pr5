FROM ubuntu:latest
# FROM openjdk:17-jdk-slim
# openjdk-17-jre \

# RUN apt-get update && apt-get install -y \
# x11-apps \
# xauth \
# openjdk-17-jre \
# && rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get install -y \
    x11-apps \
    xauth \
    openjdk:15-jdk \
    && rm -rf /var/lib/apt/lists/*



ENV DISPLAY=host.docker.internal:0

COPY calc.jar .

CMD ["java", "-jar", "calc.jar"]