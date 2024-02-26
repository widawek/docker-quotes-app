FROM gradle:8.6.0-jdk11

WORKDIR /app

ENV POSTGRES_USER=kodilla
ENV POSTGRES_PASSWORD=kodilla
ENV POSTGRES_DB=kodilla-quotes

COPY . .

RUN gradle clean build

CMD ["java", "-jar", "build/libs/quotes-0.0.1.jar"]