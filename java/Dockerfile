FROM eclipse-temurin:21-jre
 
WORKDIR /app
 
COPY server.jar .
 
RUN groupadd -r cnet && useradd -r -g cnet cnet \
    && chown -R cnet:cnet /app
 
USER cnet
 
EXPOSE 7860
 
ENTRYPOINT ["java", "-jar", "server.jar"]
