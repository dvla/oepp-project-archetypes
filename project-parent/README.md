project-parent
========

This `pom.xml` provides Maven configuration which covers:
- common test dependencies declaration
- configuration for compile and test plugins
- configuration for reporting plugins
- quality profile for applying code quality metrics

## Requirements

 * Java JDK 1.8+
 * Maven 3+

## Build

To build this project execute the following command:

```bash
  mvn clean install
```

## Profiles

### quality

Project provides quality profile which contains configuration for:
- code styling check (Checkstyle plugin)
- code analyzers (PMD + Findbugs plugins)

To run code analysis during project build please execute following command:

```bash
  mvn clean verify -P quality
```

To generate Maven quality report please execute following command:

```bash
  mvn site -P quality
```