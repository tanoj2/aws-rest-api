# REST API with API Gateway and Lambda

This repository contains the code for a REST API implemented using AWS API Gateway, Lambda functions, and SQLAlchemy for connecting to an RDS database. The API allows performing CRUD operations on the database.

## Description

The REST API is built on AWS infrastructure. The API Gateway acts as the entry point for the API, handling request routing, authorization, and rate limiting. The Lambda functions process the incoming API requests and interact with the RDS database using SQLAlchemy for performing CRUD operations.

## Prerequisites

To set up and run this project, you will need the following:

- An AWS account with appropriate permissions to create and configure API Gateway, Lambda functions, and RDS instances.
- Basic understanding of AWS services and concepts.
- Access to the AWS Management Console.

## Getting Started

To deploy and test the REST API, follow these steps:

1. Clone the repository:

2. Create an RDS database instance:

- Open the AWS Management Console.
- Navigate to the Amazon RDS service.
- Create a new database instance with the desired settings.
- Note down the database connection details (host, database name, username, and password).

3. Create a new Lambda function:

- Open the AWS Management Console.
- Navigate to the AWS Lambda service.
- Create a new Lambda function from scratch.
- Configure the function with the desired runtime and settings.
- Copy the code from the repository's Lambda function files into the function's code editor.
- Update the code with the RDS database connection details.

4. Create an API Gateway:

- Open the AWS Management Console.
- Navigate to the Amazon API Gateway service.
- Create a new API.
- Configure the API endpoints, methods, and integration settings.
- Connect the endpoints to the respective Lambda functions.

5. Deploy the API:

- In the API Gateway console, deploy the API to a stage (e.g., "dev" or "prod").
- Note down the API base URL.

6. Test the API:

- Use a tool like Postman or cURL to send HTTP requests to the API endpoints.
- Refer to the API documentation for details on the available endpoints and request/response formats.

7. Make improvements or add new features:

- Feel free to modify the code and add additional functionality as needed.
- Push your changes to the Git repository to track your progress and collaborate with others.

## API Documentation

### Endpoint 1: [GET] /resources

Returns a list of all resources.

### Endpoint 2: [POST] /resources

Creates a new resource using the provided data.

### Endpoint 3: [PUT] /resources/{id}

Updates an existing resource with the provided ID.

### Endpoint 4: [DELETE] /resources/{id}

Deletes a resource with the provided ID.


