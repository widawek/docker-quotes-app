FROM gradle:8.6.0-jdk11

WORKDIR /app

ENV SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/kodilla-quotes
ENV SPRING_DATASOURCE_USERNAME: kodilla
ENV SPRING_DATASOURCE_PASSWORD: kodilla

COPY . .

RUN gradle clean build

CMD ["java", "-jar", "build/libs/quotes-0.0.1.jar"]