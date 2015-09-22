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

## Build

To build this project execute the following command:

```bash
  mvn clean install
```