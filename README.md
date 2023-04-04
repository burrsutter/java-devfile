# Java, Quarkus, Hello, with Dockerfile

### Java with Devfile no Dockerfile reference

The following commands only work if you fix the syntax error left in place purposefully for demo purposes

```
mvn package

java -jar target/quarkus-app/quarkus-run.jar

curl localhost:8080

Hello Quarkus 4 12-23-2022 03:13:59 on unknown
```

```
docker build -f src/main/docker/Dockerfile.jvm -t java-devfile .

docker run -i --rm -p 8080:8080 java-devfile

curl localhost:8080

Hello Quarkus 1 12-24-2022 03:39:03 on e29c6975f9e3
```