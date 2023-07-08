web: java -Dserver.port=$PORT -jar target/demo-0.0.1-SNAPSHOT.jar  --spring.profiles.active=prod, heroku,no-liquibase 
release: cp -R src/main/resources/config config && ./mvnw -ntp liquibase:update -Pprod,heroku
