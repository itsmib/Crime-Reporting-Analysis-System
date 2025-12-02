# Crime Reporting Analysis System

A Java-based command-line application for reporting and analyzing crime data. The system stores crime information in a MySQL database and allows adding, viewing, searching, updating, and deleting crime records.

---

## 🚀 Features

- Add new crime reports  
- View all crime records  
- Search by category, date, or location  
- Update crime entries  
- Delete crime entries  
- Simple analytics (counts by category/location)  
- JDBC-based MySQL connectivity  
- Maven dependency management  
- JUnit test cases  

---

## 🛠️ Tech Stack

- Java (JDK 11+)  
- MySQL  
- Maven  
- JDBC  
- JUnit  

---

## 📂 Project Structure

    CrimeReportingSystem/
        src/
            main/
                java/
                    dao/                (Database access classes)
                    model/              (POJO classes: Crime, User, Location)
                    service/            (Business logic: CrimeService, Validation)
                    Main.java           (CLI entry point)
            test/
                java/                   (JUnit test cases)
        sql/
            schema.sql                  (Database tables & initial setup)
        resources/
            application.properties       (DB credentials if used)
        pom.xml                          (Maven config)
        README.md                        (This file)

---

## 🗄️ Database Setup

1. Create database:

       CREATE DATABASE crime_db;

2. Run schema:

       mysql -u root -p crime_db < sql/schema.sql

3. Update DB credentials inside the project:

       URL      → jdbc:mysql://localhost:3306/crime_db
       USER     → root
       PASSWORD → your_password

---

## ▶️ How to Build & Run

Build:

    mvn clean package

Run:

    java -jar target/crime-reporting-system.jar

Run tests:

    mvn test

---

## 🤝 Contributing

1. Fork the project  
2. Create a branch  
3. Commit changes  
4. Open a pull request  

---

## 📄 License

Add a LICENSE file as needed.
