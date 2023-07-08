web: java $JAVA_OPTS -Xmx256m -jar target/*.jar --spring.profiles.active=prod,  java -Dserver.port=$PORT -jar target/demo-0.0.1-SNAPSHOT.jar, heroku,no-liquibase 
release: cp -R src/main/resources/config config && ./mvnw -ntp liquibase:update -Pprod,heroku
