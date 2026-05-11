# Dockerized Shopping Web App

## Overview

This project is a containerized version of a Node.js shopping web application using Docker and Docker Compose. It integrates a Node.js backend with a MongoDB database running in separate containers, communicating through a custom Docker network.

The main goal of this project is to demonstrate how a full-stack application can be containerized and managed using Docker.

---

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Docker
- Docker Compose

---

## Features

- Fully containerized backend and database
- Multi-container setup using Docker Compose
- Service communication using Docker networking
- MongoDB running in a separate container
- Environment-based configuration support
- Persistent backend-database communication

---

## Architecture
Frontend (if any) / Browser
|
v
Node.js Application Container
|
v
MongoDB Container
|
Docker Network (bridge)


---

## How to Run the Project

### Using Docker Compose

```bash
docker compose up --build
```

## Access Application
http://localhost:3000

## Environment Variables
MONGO_DB=shop
PORT=3000

## Notes
- MongoDB runs in a separate container and communicates via Docker service name (db)
- Application and database are connected through a custom Docker bridge network
- Ensure ports 3000 and 27017 are not blocked locally
