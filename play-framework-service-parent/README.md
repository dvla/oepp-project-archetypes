play-framework-service-parent
========

This `pom.xml` provides Maven configuration for standard Play Framework (www.playframework.com) based applications.

This `pom.xml` file:
- allows building Play Framework application with Maven
- enables RPM building plugin (with default configuration)

## Requirements

 * Java JDK 1.8+
 * Maven 3+

## Configure
You need to ensure that the `play-framework-service.port` property is defined in your maven settings. Please refer the `README.md` file of the parent project for how to do this.

## Build

To build this project execute the following command:

```bash
  mvn clean install
```