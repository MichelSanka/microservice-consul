FROM openjdk:11.0.2-jre-slim
COPY target/microservice-consul-demo-order-0.0.1-SNAPSHOT.jar .
COPY nudge-agent/nudge-4.0.3.jar .
COPY nudge-agent/nudge.properties .
CMD /usr/bin/java -Dlogging.path=/log/ -Xmx400m -Xms400m -javaagent:nudge-4.0.3.jar -jar microservice-consul-demo-order-0.0.1-SNAPSHOT.jar
EXPOSE 8080
