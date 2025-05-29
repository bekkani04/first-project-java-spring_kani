# First Project Java Spring

Educational Spring Boot project with web interface and Thymeleaf templating engine.

## Description

This is a first Java Spring Boot project created for learning web development fundamentals. The project includes:

- Spring Boot 3.4.5
- Spring Web for creating REST APIs and web controllers
- Thymeleaf for HTML template rendering
- Apache Maven for dependency management

## Technologies

- **Java** - main programming language
- **Spring Boot 3.4.5** - framework for creating web applications
- **Spring Web** - module for web development
- **Thymeleaf** - template engine for HTML generation
- **Apache Maven** - project build system

## Requirements

- Java 17 or higher
- Apache Maven 3.6+

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/username/first-project-java-spring.git
cd first-project-java-spring
```

### 2. Build the project

```bash
mvn clean install
```

### 3. Run the application

```bash
mvn spring-boot:run
```

Or run the JAR file:

```bash
java -jar target/first_project_java_spring-0.0.1-SNAPSHOT.jar
```

### 4. Open in browser

Navigate to: `http://localhost:8080`

## Functionality

### URL Parameter Handling

The application supports passing parameters through URL address. Parameters are automatically displayed on the web page.

**Usage example:**
```
http://localhost:8080?name=John&age=25
```

The passed parameters will be displayed on the website screen.

### Screenshots

![Main Page](images/Screenshot(365).png)

## Project Structure

```
src/
├── main/
│   ├── java/
│   │   └── pl/edu/vistula/first_project_java_spring/
│   │       ├── FirstProjectJavaSpringApplication.java
│   │       └── controller/
│   └── resources/
│       ├── templates/          # Thymeleaf templates
│       ├── static/            # CSS, JS, images
│       └── application.properties
└── test/
    └── java/
```

## Useful Commands

### Build without tests
```bash
mvn clean package -DskipTests
```

### Create Docker image
```bash
mvn spring-boot:build-image
```

### Run tests
```bash
mvn test
```

## API Endpoints

Documentation for available endpoints will be added as the project develops.

## Development

### Adding new dependencies

Add required dependencies to `pom.xml` and run:

```bash
mvn clean install
```

### Hot reload

To enable automatic reload during development, add to `pom.xml`:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
    <scope>runtime</scope>
    <optional>true</optional>
</dependency>
```

## Useful Links

- [Spring Boot Documentation](https://docs.spring.io/spring-boot/3.4.5/reference/)
- [Spring Web Guide](https://docs.spring.io/spring-boot/3.4.5/reference/web/servlet.html)
- [Thymeleaf Documentation](https://www.thymeleaf.org/documentation.html)
- [Apache Maven Guide](https://maven.apache.org/guides/index.html)

## Notes

⚠️ **Important**: The original package name `pl.edu.vistula.first-project-java-spring` was changed to `pl.edu.vistula.first_project_java_spring` due to Java package naming restrictions.

## License

Educational project. No license specified.

## Author
Kanykei Beksultanova
