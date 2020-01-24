FROM openjdk:8-jdk-slim

ADD entrypoint.sh entrypoint.sh
ADD build/libs/gs-serving-web-content-0.1.0.jar app.jar
RUN apt update && \
    apt install -y curl && \
    chmod +x entrypoint.sh
CMD ["./entrypoint.sh"]
