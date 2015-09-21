service-parent
========

Project provides Maven configuration which covers:
- configuration for JAR building plugins
- release profile for building RPM packages

## Requirements

 * Java JDK 1.8+
 * Maven 3

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
  mvn clean package -P release -Dgpg.keyPassphrase=[GPG key passphrase]
```