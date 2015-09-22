dropwizard-service-parent
========

This `pom.xml` provides Maven configuration for standard Dropwizard (www.dropwizard.io) based services.

This `pom.xml` file:
- declares base service dependencies (including Swagger API dependencies)
- enables JAR building and dependency copying plugins
- enables RPM building plugin (with default configuration)

## Requirements

 * Java JDK 1.8+
 * Maven 3+

## Build

To build this project execute the following command:

```bash
  mvn clean install
```