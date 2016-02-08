project-archetypes
========

Project provides set of parent `pom.xml` files with base configuration for other projects:

 * project-parent (see: [README](project-parent))
 * service-parent (see: [README](service-parent))
 * dropwizard-service-parent (see: [README](dropwizard-service-parent))
 * play-framework-service-parent (see: [README](play-framework-service-parent))

Additionally project-archetypes `pom.xml` also contains configuration for dependency and distribution management repositories.

## Requirements

 * Java JDK 1.8+
 * Maven 3+

## Configure

You need to add some properties to your maven `settings.xml` file (this is usually located in the `.m2` folder in your home directory).
Here is a sample settings.xml with the properties in it, populated with dummy values that you need to change:

```bash
<?xml version="1.0" encoding="UTF-8"?>

<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
http://maven.apache.org/xsd/settings-1.0.0.xsd"

    <profiles>
        <profile>
            <id>oepp-properties</id>
            <properties>
                <source-code-repository.url>your source code repository url (e.g. https://localhost/git)</source-code-repository.url>
                <binary-repository-manager.url>your binary repository manager url (e.g. https:localhost/nexus)</binary-repository-manager.url>
                <dropwizard-service.port>default dropwizard service port (e.g. 8080))</dropwizard-service.port>
                <play-framework-service.port>default play framework port (e.g. 9000)</play-framework-service.port>
            </properties>
        </profile>
    </profiles>
    <activeProfiles>
        <activeProfile>oepp-inject-properties</activeProfile>
    </activeProfiles>
</settings>
```

## Build

To build this project execute the following command:

```bash
  mvn clean install
```