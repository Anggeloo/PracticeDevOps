# PHP Hello World Web Application

This is a simple PHP web application that displays a "Hello World" message and a personal introduction.

## Prerequisites

* PHP 7.4 or higher
* Docker (if running with containers)
* Git

## Getting Started

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/Anggeloo/PGM1.git
```

2. Change to the project directory:
```bash
cd PGM1
```

3. If you have PHP installed locally, you can run:
```bash
php -S localhost:8080
```

### Running with Docker

1. Build the Docker image:
```bash
docker build -t pgm1 .
```

2. Run the Docker container:
```bash
docker run -p 8080:8080 pgm1
```

The application will be available at http://localhost:8080

## Project Structure

* `PGM1.php`: The main application file containing the HTML and PHP code that displays the Hello World message
* `Dockerfile`: Configuration file for building the Docker container with PHP 7.4

## Dockerfile Details

The Dockerfile:
* Uses PHP 7.4 CLI base image
* Copies the PHP file to the container
* Renames it to index.php
* Exposes port 8080
* Runs a PHP development server

## Accessing the Deployed Application

The application is deployed on Render and can be accessed at:
https://pgm1.onrender.com

## Technologies Used

* PHP 7.4
* Docker
* HTML
* Render (for deployment)
