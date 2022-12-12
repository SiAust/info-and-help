# Springboot tips

### Basics

- `./gradlew bootRun` = run a Springboot Gradle project
- `./mvnw spring-boot:run` = run a Springboot Maven project
  - `-e` = extra log info for errors

## General

- `log.info("hello {}", name)` = `{}` placeholder for variable in string (I think multiple placeholders work based on
  given argument order)
- `/h2-console/<database name>` = default path in URL for H2 console
- `ctrl + c` = kill app from console
- `http://localhost:8080/actuator/shutdown` = goto url to shutdown (must be enabled in settings)
- `endpoints.shutdown.enabled = true` = `application.properties` setting to allow endpoint shutdown (above)
