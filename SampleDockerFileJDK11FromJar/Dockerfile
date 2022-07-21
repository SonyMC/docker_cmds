# Create an Image from a supplied jar file
FROM openjdk:11-jre-slim
VOLUME /tmp
COPY netflix-eureka-naming-server-v2-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8761
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]