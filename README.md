## Running the Application:

Ensure MongoDB is Running Locally:

    cd src/docker
    docker-compose up -d

Make sure you have MongoDB installed and running on your local machine or run it via docker. 

By default, MongoDB runs on localhost:27017.

# Run the Spring Boot Application:

- Open a terminal and navigate to the directory containing your pom.xml.
- Run the application using Maven


    ./mvnw spring-boot:run


## Testing the Application:

You can test the REST API using tools like curl or Postman.

# Get all users:

    curl -X GET http://localhost:8080/users

# Create a new user:

    curl -X POST http://localhost:8080/users -H "Content-Type: application/json" -d '{"name": "John Doe", "email": "john.doe@example.com"}'

# Get user by ID:

    curl -X GET http://localhost:8080/users/{id}

# Update a user:

    curl -X PUT http://localhost:8080/users/{id} -H "Content-Type: application/json" -d '{"name": "Jane Doe", "email": "jane.doe@example.com"}'

# Delete a user:

    curl -X DELETE http://localhost:8080/users/{id}

