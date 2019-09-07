# Quarkus

https://code.quarkus.io/

# Build & Run

mvn compile quarkus:dev -Dquarkus.http.port=9000


# Build Docker

mvn package

docker build -f src/main/docker/Dockerfile.jvm -t quarkus/code-with-quarkus-jvm .

docker run -i --rm -p 8080:8080 quarkus/code-with-quarkus-jvm
