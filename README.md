# Heavy Load Management Project

## Description

This project demonstrates how to generate 10 million records of fake data using the **Java Faker** library, insert them into a PostgreSQL database, and export the data to a CSV file. The goal is to simulate the insertion of large amounts of data into a database and facilitate its export for further analysis.

## Features

- **Data Generation**: Uses **Java Faker** to generate fake data for `Person` records (ID, Name, Email, Address, Age).
- **Database Insertion**: Inserts the generated data into a PostgreSQL database using **JDBC**.
- **CSV Export**: Exports the generated data into a CSV file, allowing easy access to the records outside the database.
- **Batch Processing**: Uses batch inserts for better performance when inserting large amounts of data into the database.

## Prerequisites

Before running the project, ensure you have the following installed:

- **JDK 8 or higher**: [Download](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)
- **PostgreSQL**: [Download](https://www.postgresql.org/download/)
- **Maven** (optional, if you're using Maven for dependency management): [Download](https://maven.apache.org/download.cgi)

### Dependencies

- **Java Faker**: For generating fake data.
- **PostgreSQL JDBC Driver**: For connecting Java to the PostgreSQL database.
- **OpenCSV**: For writing the generated data to a CSV file.

If you are using **Maven**, the dependencies are already included in the `pom.xml`.

### Maven Dependencies
```xml
<dependencies>
    <dependency>
        <groupId>com.github.javafaker</groupId>
        <artifactId>javafaker</artifactId>
        <version>1.0.2</version>
    </dependency>
    <dependency>
        <groupId>com.opencsv</groupId>
        <artifactId>opencsv</artifactId>
        <version>5.6</version>
    </dependency>
</dependencies>
