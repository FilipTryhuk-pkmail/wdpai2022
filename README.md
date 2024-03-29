# GoldenOaks

GoldenOaks is a web app to manage and track your book collection. See what others are reading and exchange your books with them!

## Table of Contents

* [Technologies](#technologies)
* [Documentation](#documentation)
* [Database](#database)

## Technologies
Technologies used in the project:
* HTML 5
* CSS
* PHP (version 7.4.3 or newer)
* JavaScript
* PostgreSQL

## Documentation

### public/css
* headers.css -- styling the logo and the page selection bar
* style.css -- default styling for non-specific pages
* history.css -- styling for the book exchange history page
* logout.css -- styling the logout page
* register.css -- styling the registration form
* book_cover.css -- styling the cover upload form
* book_display.css -- styling the book collection page

### public/css
Contains logos and default images used by the site.

### public/js
* script.js -- handles email validation
* search.js -- handles managing the book database

### public/views
* books.php -- shows available books and allows searching for specific titles/authors
* history.php -- displays the last book exchanges
* login.php -- allows the user to log in
* logout.html -- displays a message after logging out
* bookcover.php -- allows uploading cover images for books
* register.php -- lets the user register a new account 

### public/src/controllers
* AppController.php -- base controller class, inherited by all other controllers
* SecurityController.php -- handles the backend management of user accounts and sessions
* DefaultController.php -- default app controller
* BookController.php -- controls operations on books in the database
* BookCoverController.php -- backend image file upload and validation

### public/src/models
* Book.php -- provides methods and fields necessary for handling Book objects
* User.php -- provides methods and fields necessary for handling User objects
* BookCover.php -- provides methods and fields necessary for handling BookCover objects

### public/src/repository
* Repository.php -- base Repository class, inherited by the other repository classes
* UserRepository.php -- repository management for User objects
* BookRepository.php -- repository management for Book objects

### Database.php
Contains the script used to connect to the database server.

### Routing.php
Contains app routing for GET, POST and RUN functions, includes all Controllers.

### docker-compose.yml
Docker configuration file.

### index.php
Responsible for parsing urls into GET and RUN functions, handled by chosen Controllers.

## Database
Database used by the app has been exported into the script.sql file available in the main directory of the repository.
