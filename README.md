# Golang-CRUD-API-using-FIBER-and-MySQL-with-GORM
A Simple Golang CRUD API example using the Fiber framework and GORM to interact with a MySQL database.
To run:
1. open the integrated terminal in your IDE or text editor and start the MySQL server in Docker by running the command ```docker-compose up -d```
2. After that, run the command ```go run main.go``` in the terminal to install the necessary packages, migrate the GORM schema to the MySQL database, and start the Fiber HTTP server.
3. To test the CRUD endpoints, you can import the ```Note App.postman_collection.json``` file into Postman and make HTTP requests to the Fiber server. 
    Alternatively, you can set it up with your own front end.