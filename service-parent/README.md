service-parent
========

This `pom.xml` provides Maven configuration which covers:
- configuration for JAR building and dependency copying plugins
- release profile for building RPM packages

Because this module is very generic by design, none of the plugins are enabled by default. Modules which use this `pom.xml` should enable them when needed.

## Requirements

 * Java JDK 1.8+
 * Maven 3+

## Build

To build this project execute the following command:

```bash
  mvn clean install
```

## Profiles

### release

Project provides release profile which packages services into deployable RPM packages.

To build RPM package please execute following command:

```bash
  mvn clean package -P release
```