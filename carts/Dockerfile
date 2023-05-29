FROM amazoncorretto:8-alpine

RUN apk update && apk add stress-ng --no-cache

WORKDIR /usr/src/app
COPY app.jar ./app.jar

ENTRYPOINT ["java", "-jar", "./app.jar", "--port=80"]
