# online-ticket-booking

This project is a **Full Stack Online Ticket Booking System** containerized using **Docker** and deployed using **Kubernetes**.  
It allows users to browse available events, book tickets, and manage their bookings.

> **Note:** This repository is structured, containerized, and configured for Kubernetes deployment.

---

## Tech Stack

| Layer | Technology Used |
|------|----------------|
| Frontend | (EDIT THIS) React / Angular / HTML-CSS-JS |
| Backend | (EDIT THIS) Node.js / Spring Boot / Django / Flask |
| Database | (EDIT THIS) MySQL / MongoDB / PostgreSQL |
| Containerization | Docker |
| Orchestration | Kubernetes |
| Load Balancing / Routing | Kubernetes Ingress |


---

## Features

- User Login & Authentication
- Event / Show / Movie listing
- Ticket booking & confirmation
- Secure backend API routes
- Supports scaling using Kubernetes replicas

---

## Docker Setup

### Build the images:

docker build -t ticket-frontend ./frontend
docker build -t ticket-backend ./backend


### Run locally (optional):

docker run -p 3000:3000 ticket-frontend
docker run -p 5000:5000 ticket-backend

### Apply all deployment & service files:

kubectl apply -f k8s-deployments/
