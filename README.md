📚 Library Management System

A Spring Boot RESTful API for managing books in a library .
It allows users to add , view , update and delete books using REST APIs .
This project is built to demonstrate Spring Boot + JPA + MySQL integration .

🚀 Features

  - Add new books to the library
  - View all books or a specific book by ID
  - Update book details
  - Delete a book
  - Integrated with MySQL database
  - API tested with Postman

🛠 Tech Stack

- Backend : Java , Spring Boot
- Database : MySQL ( via JPA / Hibernate )
- Tools : Spring Tool Suite ( STS ) , Maven , Git , Postman

⚙️ Project Setup

  1 . Clone Repository
      git clone https://github.com/<your-username>/Library-Management-System.git
      cd Library-Management-System

  2 . Configure Database
       Update src/main/resources/application.properties :
   
       spring.datasource.url=jdbc:mysql://localhost:3306/library_management_system?createDatabaseIfNotExist=true
       spring.datasource.username=root
       spring.datasource.password=root
       spring.jpa.hibernate.ddl-auto=update

  3 . Run the Project

      mvn spring-boot:run

  or run LibraryManagementSystemApplication.java from STS/IntelliJ.

  Server starts on :
    👉 http://localhost:8082

📌 API Endpoints

| Method | Endpoint      | Description         | Example Body (JSON)                                                  |
| ------ | ------------- | ------------------- | -------------------------------------------------------------------- |
| POST   | `/books`      | Add a new book      | `{ "title": "The Guide", "author": "R.K. Narayan", "price": 250 }`   |
| GET    | `/books`      | Get all books       | -                                                                    |
| GET    | `/books/{id}` | Get book by ID      | -                                                                    |
| PUT    | `/books/{id}` | Update book details | `{ "title": "Updated Title", "author": "New Author", "price": 300 }` |
| DELETE | `/books/{id}` | Delete a book by ID | -                                                                    |
  
