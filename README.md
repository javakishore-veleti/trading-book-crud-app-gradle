# trading-book-crud-app-gradle
trading-book-crud-app-gradle is a Spring Boot application featuring full CRUD operations for managing trading books. Built with Gradle, it leverages Spring Data JPA and Hibernate for data persistence, using an H2 in-memory database for streamlined development and testing. Ideal for exploring Spring Boot and Gradle integration.

## Project Setup Commands

### Step 01 - Executed this command to create this project structure

- Observe for
    -- Java Version = 21
    -- baseDir = trading-book-crud-app-gradle
    -- packageName = com.jk.research.trading_app
    -- name = trading-book-crud-app
    -- -0 = trading-book-crud-app-gradle.zip

```shell
curl https://start.spring.io/starter.zip \
  -d dependencies=web,data-jpa,h2 \
  -d type=gradle-project \
  -d baseDir=trading-book-crud-app-gradle \
  -d packageName=com.jk.research.trading_app \
  -d name=trading-book-crud-app \
  -d javaVersion=21 \
  -o trading-book-crud-app-gradle.zip
unzip trading-book-crud-app-gradle.zip -d trading-book-crud-app-gradle
cd trading-book-crud-app

```

### Step 02 - Building the project

```shell

./gradlew build

```

### Step 03 - Running the Spring Boot Application

```shell

./gradlew bootRun

```

### Step 04 - Access the Application

```shell

curl http://localhost:8080

```

### Additional Gradle Commands

```shell
# Clean the build directory: This command deletes the build directory to ensure a fresh build.
./gradlew clean

# Run unit tests: To run tests without building the entire project.
./gradlew test

# Build the project without running tests: If you want to skip tests during the build process.
./gradlew build -x test

```

### Running with Different Profiles
```shell
./gradlew bootRun -Pprofile=dev

# Windows 
# gradlew.bat bootRun -Pprofile=dev

```

### Adding More Custom Gradle Tasks (Optional)
```shell
./gradlew bootRunDev

# or 
./gradlew bootRunProd

```