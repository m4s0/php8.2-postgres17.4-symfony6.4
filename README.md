# PHP, Postgres, Symfony with Docker Template

A development environment template using PHP 8.2, PostgreSQL 17.4, and Symfony and Docker.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Development](#development)
- [Testing and Quality](#testing-and-quality)

## Prerequisites

- Docker
- Docker Compose
- Make

## Getting Started

Set up environment variables:
```bash
cp .env.dist .env
```
Configure `.env` file with your settings

## Development

### Container Management

Build containers:
```bash
docker-compose build
```

Start containers:
```bash
docker-compose up -d
```

Stop containers:
```bash
docker-compose down
```

### Access PHP container:
```bash
make bash
```

### Application Setup

Install dependencies:
```bash
make install
```
### Database Management

Run migrations:
```bash
make run-migrations
```

## Testing and Quality  

### Run Tests
```bash
make tests
```

### Coding Standards
```bash
make cs
```

### Static Analysis
```bash
make stan
```
