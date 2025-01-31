**FastAPI Factorial API**

**Overview**

This repository contains a simple API developed using FastAPI that computes the factorial of a given number. The API provides a single endpoint that takes an integer as input and returns the computed factorial. If the input value is 0, the API returns {"result": false}.

Features

**Developed using FastAPI.**

Uses a while loop to compute the factorial.

Returns a JSON response with the factorial result.

Handles edge cases like zero input.

**Installation**

To set up and run this FastAPI application, follow these steps:

Prerequisites

Python 3.8 or later

pip (Python package installer)

Steps

**Clone the repository:**

git clone https://github.com/yourusername/your-repository.git
cd your-repository

Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate     # On Windows

**Install dependencies:**

```pip install -r requirements.txt```

Running the Application

**Start the FastAPI server:**

```uvicorn main:app --reload```

Open your browser or use a tool like Postman to test the API at:

http://127.0.0.1:8000/factorial/{starting_number}

Replace {starting_number} with any integer value to compute its factorial.

API Endpoint

```GET /factorial/{starting_number}```

**Request:**

starting_number: Integer value whose factorial is to be computed.

Response:

If starting_number > 0:

{
  "number": 5,
  "factorial": 120
}

If starting_number == 0:

{
  "result": false
}

Dependencies

This project requires the following dependencies, listed in requirements.txt:

FastAPI

Uvicorn

Testing

You can test the API using the built-in Swagger UI provided by FastAPI:

Open http://127.0.0.1:8000/docs in your browser.

Try the GET /factorial/{starting_number} endpoint.

Author

[[Guiller Neri] - Your GitHub Profile](https://github.com/neri-Guiller09)
