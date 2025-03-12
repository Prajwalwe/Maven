# Apache Maven

## Overview
Apache Maven is a build automation and project management tool used primarily for Java projects. It simplifies dependency management, builds, and deployments using a standardized approach.

## Features
- Automated dependency management
- Build lifecycle management
- Standardized project structure
- Integration with various IDEs
- Supports multi-module projects
- Plugin extensibility

## Installation
### Prerequisites
- Java Development Kit (JDK) installed (JDK 8 or higher)
- Set `JAVA_HOME` environment variable

### Steps
1. Download Maven from the [official website](https://maven.apache.org/download.cgi).
2. Extract the archive.
3. Set `MAVEN_HOME` environment variable.
4. Add `MAVEN_HOME/bin` to the system `PATH`.
5. Verify installation:
   ```sh
   mvn -version
   ```

## Project Structure
```
my-app/
|-- src/
|   |-- main/java/ (Source Code)
|   |-- test/java/ (Test Cases)
|-- target/ (Compiled Output)
|-- pom.xml (Project Configuration)
```

## Basic Commands
| Command | Description |
|---------|-------------|
| `mvn clean` | Removes compiled files. |
| `mvn compile` | Compiles source code. |
| `mvn test` | Runs unit tests. |
| `mvn package` | Creates a JAR/WAR package. |
| `mvn install` | Installs package in local repository. |
| `mvn deploy` | Deploys package to a remote repository. |

## Adding Dependencies
Modify `pom.xml` to include dependencies:
```xml
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-core</artifactId>
    <version>5.3.10</version>
</dependency>
```

## License
This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

