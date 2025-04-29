# Simple Time Service

This is a simple Flask-based web service that provides the current UTC timestamp and the IP address of the client making the request.

## Features

- Returns the current UTC timestamp in ISO 8601 format.
- Returns the IP address of the client making the request.

## Requirements

- Python 3.9 or higher
- Flask

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd simple-time-service
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python app.py
   ```

4. Access the service at `http://localhost:5000`.

## Docker Instructions

1. Build the Docker image:
   ```bash
   docker build -t simple-time-service .
   ```

2. Run the Docker container:
   ```bash
   docker run -p 5000:5000 simple-time-service
   ```

3. Access the service at `http://localhost:5000`.

## API Endpoint

### `GET /`

- **Description**: Returns the current UTC timestamp and the client's IP address.
- **Response**:
  ```json
  {
    "timestamp": "2023-01-01T00:00:00Z",
    "ip": "127.0.0.1"
  }
  ```

## License

This project is licensed under the MIT License.
