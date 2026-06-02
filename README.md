# AFL-2 Microservices Development - All About Docker Desktop


## Project Description

This project is a simple web application featuring registration, login, and a dashboard. The application is built using Python Flask and uses PostgreSQL as its database. The project runs via Docker Compose with multiple services: Nginx acting as a load balancer, two web app containers, and one database container.

## Application Features

- User registration with username, password, and password confirmation
- User login with username and password
- Dashboard displaying the successfully logged-in username
- Logout functionality from the dashboard

## Technologies Used

- Python Flask
- PostgreSQL
- Nginx Load Balancer
- Docker
- Docker Compose

## Microservice Structure

- `nginx`: Load balancer
- `web1`: Flask web app instance 1
- `web2`: Flask web app instance 2
- `db`: PostgreSQL database
- `postgres_data`: Docker volume for persisting database data
- `afl2_network`: Docker network for connecting the services

## Prerequisites

Ensure you have the following installed on your local machine:
- [Docker Desktop](https://docker.com)
- Git (optional, for cloning)

## How to Run the Project

1. Open your terminal in the project root directory.
2. Run the following command to build and start all services:

```bash
docker compose up --build
```

3. Once the containers are running, open your web browser and access the application at:
   ```text
   http://localhost
   ```

4. To stop the application, press `Ctrl + C` in your terminal or run:
   ```bash
   docker compose down
   ```
