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

## Advanced Gradle Features We Can Do For This Spring Boot Application Project

# Gradle Advanced Features Demo

**Gradle** is a powerful build automation tool that provides a range of advanced features to streamline and optimize the build process. This project demonstrates various advanced Gradle features, including custom tasks, multi-project builds, dependency management, build caching, and integration with CI/CD pipelines.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
  - [Custom Tasks and Plugins](#custom-tasks-and-plugins)
  - [Multi-Project Builds](#multi-project-builds)
  - [Dependency Management](#dependency-management)
  - [Build Caching](#build-caching)
  - [Incremental Builds and Compilation](#incremental-builds-and-compilation)
  - [Parallel Execution](#parallel-execution)
  - [Continuous Builds](#continuous-builds)
  - [Build Scans](#build-scans)
  - [Profile and Optimize Builds](#profile-and-optimize-builds)
  - [Integrating with Other Tools](#integrating-with-other-tools)
  - [Task Avoidance API](#task-avoidance-api)
  - [Advanced Testing with Gradle](#advanced-testing-with-gradle)
  - [Dynamic Versioning and Dependency Resolution](#dynamic-versioning-and-dependency-resolution)
- [Usage](#usage)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This repository demonstrates how to utilize advanced features of Gradle to build, test, and deploy Java applications more efficiently. Gradle provides powerful capabilities like task automation, build caching, parallel execution, and more to help developers manage complex build processes.

## Features

### Custom Tasks and Plugins

Define custom Gradle tasks to perform specific actions, such as generating documentation, running scripts, or managing resources. You can also create reusable plugins to encapsulate common build logic.

### Multi-Project Builds

Manage multiple related projects simultaneously with Gradle's support for multi-project builds. Configure subprojects from a central `settings.gradle` file.

### Dependency Management

Use advanced dependency configurations to manage dependencies with fine-grained control, lock dependencies to specific versions, and avoid conflicts.

### Build Caching

Leverage Gradle's build cache mechanism to reuse outputs from previous builds, reducing build times by avoiding unnecessary work.

### Incremental Builds and Compilation

Optimize task execution by configuring tasks to run incrementally, only executing the parts of the build that have changed since the last build.

### Parallel Execution

Enable parallel builds to build subprojects simultaneously, significantly reducing build times for large multi-project builds.

### Continuous Builds

Utilize Gradle's continuous build mode to automatically re-execute tasks when their inputs change, ideal for development environments.

### Build Scans

Generate detailed build scans to diagnose and optimize builds, providing insights into task execution times, dependencies, and more.

### Profile and Optimize Builds

Use Gradle's build profiling feature to identify bottlenecks in the build process and optimize task execution.

### Integrating with Other Tools

Integrate Gradle with CI/CD tools like Jenkins, GitHub Actions, and GitLab CI. Automate deployment tasks, run tests, or perform code quality checks.

### Task Avoidance API

Optimize task creation and execution with Gradle's Task Avoidance API, reducing the overhead of creating tasks that are never executed.

### Advanced Testing with Gradle

Configure Gradle to run tests with different testing frameworks (JUnit 5, TestNG) and support advanced test configuration like parameterized tests and test filtering.

### Dynamic Versioning and Dependency Resolution

Use dynamic versions to always use the latest patch or minor release. Customize dependency resolution strategies to handle version conflicts or substitute specific modules.

## Usage

To run this project with Gradle, use the following commands:

```bash
# Clean the build
./gradlew clean

# Build the project
./gradlew build

# Run the application
./gradlew bootRun

# Run custom tasks
./gradlew customTask

