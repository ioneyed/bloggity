# Introduction

This version of Bloggity will be created using Spring and JPA. This will demonstrate the core functionality of the application utilizing the JPA ORM system. Hopefully this will show some streamlining of code by utilizing the JPA that users will see the power in doing POC's with JPA and CRUD Applications using it (as performance permits).

## Tech Used

Spring Boot

Thymeleaf (Render initial index page)

Spring Security

JPA

H2 Database (local database engine)

## Legend

Throughout the code and in the README you will see the following snippets.

- \[Preference\] - This means that the decision to do XYZ was made by a developer preference
- \[Best Practice\] - This means that the decision to do XYZ was a best practice (still subjective therefore 'proof' should be included).


## Step 0 - Plumbing

Plumbing will happen in just about any project that you create. This is the step where we set up our h2 configuration and basic project configuration.

- \[Preference\] Application Properties Files - This file (`src/main/resources/application.properties`) is used to store configuration details such as the port you want spring boot to initialize on (`default 8080`) or how you want the application to connect to your database.
    - I personally prefer the YAML files instead of dot notation property files so I renamed the default file - `application.properties` to `application.yml`. The function the same just look different in the code used to configure the application.

- Configure H2 to use an in-memory mode so we have a fresh database each time.

