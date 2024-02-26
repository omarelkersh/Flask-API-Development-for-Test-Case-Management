# Flask API for Test Case Management

This Flask API is designed to manage test cases and their execution results across multiple test assets, with data stored in a SQLite database.

## Table of Contents

- [Project Description](#project-description)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Testing](#testing)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Project Description

The project aims to develop a Flask API that enables users to perform various operations related to managing test cases and their execution results. It includes functionalities such as creating, retrieving, updating, and deleting test cases, recording execution results, and retrieving execution results for specific test assets.

## Requirements

1. Set up a SQLite database to store test cases and their execution results with appropriate table schema.
2. Create endpoints for:
   - Creating, retrieving, updating, and deleting test cases.
   - Recording execution results of test cases for specific test assets.
   - Retrieving execution results of test cases for specific test assets.
3. Implement data validation and error handling for each endpoint.
4. Write unit tests to ensure the functionality of each endpoint.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/your_project.git
   
## Navigate to the project directory:

  ```bash
  cd your_project
  ```
## Install the required dependencies:

  ```bash
  pip install -r requirements.txt
  ```

## Usage
To run the Flask API locally, execute the following command:

  ```bash
  python api.py
  ```
The API will be accessible at http://localhost:5000.

## Endpoints
The following endpoints are available:

POST /testcases: Create a new test case.
GET /testcases: Retrieve all test cases.
GET /testcases/<test_case_id>: Retrieve a single test case by its ID.
PUT /testcases/<test_case_id>: Update an existing test case.
DELETE /testcases/<test_case_id>: Delete a test case by its ID.
POST /execute: Record the execution result of a test case for a specific test asset.
GET /execute/<test_asset>: Retrieve the execution results of all test cases for a specific test asset.

## Testing
The project includes unit tests to ensure the functionality of each endpoint. Run the tests using the following command:

  ```bash
  python test.py
  ```
## Dependencies
The project relies on the following dependencies:

Flask
Flask-SQLAlchemy
SQLAlchemy
Other dependencies listed in requirements.txt


  
