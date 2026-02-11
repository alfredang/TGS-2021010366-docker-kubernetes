# TGS-2021010366-docker-kubernetes

Hands-on Docker labs covering core concepts from basic containers to multi-service Docker Compose applications.

## Labs

| Lab | Topic | Description |
|-----|-------|-------------|
| lab1 | First Container | Run an interactive Ubuntu container |
| lab2 | Nginx | Run Nginx and write /etc/hosts to a file |
| lab3 | Python Container | Build and run a simple Python print app |
| lab3-2 | Tetris Game | Run a static web app (Tetris) with Nginx |
| lab4 | Flask App | Build a Flask web app with Docker |
| lab5 | Volumes | Persist data with named volumes |
| lab5-2 | Dockerfile Volumes | VOLUME instruction in Dockerfile |
| lab6 | Networks | Container networking and DNS |
| lab7 | Port Mapping | Host vs container ports |
| lab8 | Environment Variables | ENV in Dockerfile and runtime overrides |
| lab9 | Docker Hub | Push the Tetris game to Docker Hub |
| lab9-2 | Docker Hub | Push and pull images |
| lab10 | Docker Compose | Single service with Compose |
| lab11 | Multi-Service Compose | Flask + Redis with Compose |
| lab12 | Full-Stack Compose | Web + PostgreSQL + Redis with healthchecks |

## Tests

| Test | Description |
|------|-------------|
| test1 | Practical test covering labs 1–9 (Dockerfile, build, run, push) |
| test2 | Practical test covering labs 10–12 (WordPress with Docker Compose) |

## Getting Started

```bash
# Start with lab1
cd lab1
# Follow the instructions in lab.md
```

Each lab folder contains a `lab.md` with step-by-step commands to follow.

## Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
