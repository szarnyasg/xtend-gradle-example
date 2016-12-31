# xtend-gradle-example

This repository contains a simple project to reproduce the issue.

## To reproduce the issue

1. Clean the Git repository

  ```
  git clean -f -x -d .
  ```
1. Build the project **without the eclipse plug-in**:

  ```
  ./gradlew build
  ```
1. Start Eclipse.
1. Import the project with **Import** | **Gradle Project** using the Gradle wrapper.
1. The project will display errors for duplicate classes:

  > The type HelloWorld is already defined

## To work around the issue

1. Clean the Git repository

  ```
  git clean -f -x -d .
  ```
1. Build the project **with the eclipse plug-in**:

  ```
  ./gradlew build
  ```
1. Start Eclipse.
1. Import the project with **Import** | **Gradle Project** using the Gradle wrapper.
1. The project will work fine.
