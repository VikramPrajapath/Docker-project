# Docker Project

This project is my first experience with Docker! It utilizes **Python Flask** and **Redis** to create a simple web application that counts the number of visits to the homepage.

## Project Overview

This Dockerized project demonstrates:
- Basic Docker setup with Flask and Redis.
- Containerized application running multiple services (web and Redis) within a Docker Compose environment.
- Simple HTTP server functionality to track the number of times the webpage is visited.

## How It Works

1. **Web Application**: Built with Python Flask, this app serves a simple web page.
2. **Redis Server**: Acts as a database to store and increment the visitor count.
3. **Counter**: Each visit to the homepage increments a counter stored in Redis, showing the visit count on the web page.

## Project Structure

```
docker-project/
├── app/                      # Application source code
│   ├── app.py                # Main Flask app
│   ├── requirements.txt      # Dependencies
├── docker-compose.yml        # Docker Compose configuration
└── README.md                 # Project documentation
```

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/) installed on your machine.

## Getting Started

To run the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/VikramPrajapath/Docker-project.git
   cd docker-project
   ```

2. Build and start the Docker containers:
   ```bash
   docker-compose up --build
   ```

3. Open your browser and go to `http://localhost:5000` to see the app in action. Each refresh increments the counter.

## Technologies Used

- **Docker**: Containerization
- **Python Flask**: Web server framework
- **Redis**: In-memory data store



