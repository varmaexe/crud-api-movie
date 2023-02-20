# CRUD-API(movies)

## Overview
This project is a Golang-based API that performs CRUD (Create, Read, Update, Delete) operations on movies. The API uses the Gorilla Mux package to handle HTTP requests and routing. The API stores movie data in memory, and it does not use any database.

# Installation
To use the API, you will need to have Golang installed on your computer. You can download and install Golang from the official website: https://golang.org/dl/

Once you have Golang installed, you can clone the repository and run the following command to install the required packages:

```go
go get github.com/gorilla/mux
```

## Usage

To use the API, run the following command:
```go
go run main.go
```

This will start the server on port 8000.

You can then make HTTP requests to the API to perform CRUD operations on movies from postman.

API Endpoints
The API has the following endpoints:

GET /movies
This endpoint returns a list of all movies.

GET /movies/{id}
This endpoint returns a particular movie with requested id

POST /movies This endpoint creates a movie if we submit json in body and returns created movie

PUT /movies/{id} This endpoint updates the movie details

DELETE /movies/{id} This endpoint delete the movie

Example request:
```postman
http://localhost:8000/movies
```
This will return all the movies in JSON

```css
[{"id":1,"title":"The Shawshank Redemption","director":"Frank Darabont","year":1994},{"id":2,"title":"The Godfather","director":"Francis Ford Coppola","year":1972}]
```

## Contributing
If you would like to contribute to the project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and test them.