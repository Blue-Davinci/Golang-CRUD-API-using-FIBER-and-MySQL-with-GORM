# Golang-CRUD-API-using-FIBER-and-MySQL-with-GORM
A Simple Golang CRUD API example using the Fiber framework and GORM to interact with a MySQL database.
To run:
1. open the integrated terminal in your IDE or text editor and start the MySQL server in Docker by running the command ```docker-compose up -d```
2. After that, run the command ```go run main.go``` in the terminal to install the necessary packages, migrate the GORM schema to the MySQL database, and start the Fiber HTTP server.
3. To test the CRUD endpoints, you can import the ```Note App.postman_collection.json``` file into Postman and make HTTP requests to the Fiber server. 
    Alternatively, you can set it up with your own front end.

# How to Build
1. Make your own directory and mod init it
```
mkdir golang-fiber-mysql
cd golang-fiber-mysql
go mod init github.com/wpcodevo/golang-fiber-mysql
```
2. Initialize packages
```
go get github.com/gofiber/fiber/v2
go get github.com/google/uuid
go get github.com/go-playground/validator/v10
go get -u gorm.io/gorm
go get gorm.io/driver/mysql
go get github.com/spf13/viper
go install github.com/cosmtrek/air@latest
```
--The packages are used for the following:
```
fiber – A high-performance web framework for Golang that supports middleware, routing, and error handling, as well as many other features commonly found in web frameworks.
uuid – A library to generate and parse UUIDs in Golang.
validator – A library for validating Go structs, values, and variables.
gorm – Provides a rich set of features such as automatic database schema generation, association handling, and query building, making it a popular choice for building web applications and services in Go.
mysql – A MySQL driver for GORM
viper – A library for managing configuration files in Golang.
air – This library automatically rebuilds and restarts your application.
```
3. You can use go's cli or air tool to run start the server and check it's health and correctness by running ```http://localhost:8000/api/healthchecker``` on your browser.
