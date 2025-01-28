The Bookstore API is a simple RESTful service designed to manage books in a database. 
It allows users to perform basic CRUD (Create, Read, Update, Delete) operations on book records. 
Each book contains details such as the name, author, and publication.

Features

Create a Book: Add a new book to the database.     
Read Books: Retrieve a single book or a list of all books.    
Update a Book: Modify an existing book's details.      
Delete a Book: Remove a book from the database.

Each book includes:

id: Unique identifier for the book.      
name: Title of the book.    
author: Author of the book.     
publication: Publication

Setup and Installation

Clone the repository:     
git clone https://github.com/Joshdike/bookstore.git        
cd bookstore

Install Go:     
If you don’t have Go installed, download and install it from the official website: https://golang.org/dl/.

Set up the database:    
Install and configure your database.       
Update the database connection details in the .env file

Install dependencies:     
Use Go modules to install dependencies:     
go mod download       
Run database migrations      
migrate -path ./migrations -database "your-database-url" up

Run the application:

go run main.go

Access the API:

The API will be running at the port specified in your configuration.

Environment Variables     
Create a .env file in the root directory with the following variables:
PORT= your specified port, 
DB_HOST=localhost,
DB_PORT=5432,
DB_USER=your_db_user,
DB_PASSWORD=your_db_password,
DB_NAME=bookstore

Technologies Used

Database: PostgreSQL         
Other Tools: Docker

Contributing         
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
