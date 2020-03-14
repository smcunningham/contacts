###ABOUT
CONTACTS is a simple web application that displays a contact list, with the contacts fetched from a PostgreSQL database. In order to connect to the database the `sqlx` and `pgx` packages were used. 
Templates were utilized to display the data on the webpage.

###HOW TO USE
##Create your database (PostgreSQL) using the `contacts.sql` file included in the `db` directory. Importing it should create the table and fake data.

Find the 'Connection String` in your database hosting software; you will need this to connect the application.

##Determine how you will run the application; do you want to pass in a `-conn` variable via the CLI, or will you create a `.env` file that the program will automatically detect and use when booting?

#CLI
In a terminal pointing to your root directory, type `go run main.go -conn "connection string here"`

#Using Environmental Variables
Create a `.env` file in your root directory. Add two variables in the file:
DATABASE_URL="your connection string here"
LISTENADDR=:"Enter an open port (default is :8080)"

In a terminal pointing to your root directory, type `go run main.go`

##Navigate to `http://localhost:8080`, or whichever port you chose to serve the application on.

Enjoy!
