# CRUD API with Validation & Database

NestJS API with DTO validation, error handling, PostgreSQL, and Docker.

## Features

- DTO validation with class-validator
- Global exception handling
- PostgreSQL with TypeORM
- User CRUD operations
- Unit tests
- Dockerized

## Setup

1. Clone the repo
2. Copy `.env.example` to `.env`
3. Install dependencies:
```bash
   npm install
```

## Run Locally
```bash
docker-compose up postgres -d


npm run start:dev
```

## Run with Docker
```bash
docker-compose up
```

## Test
```bash

npm test

npm run test:e2e

npm run test:cov
```

## API Endpoints

- `POST /users` - Create user
- `GET /users` - Get all users
- `GET /users/:id` - Get user by ID
- `PATCH /users/:id` - Update user
- `DELETE /users/:id` - Delete user

## Example Request
```bash
curl -X POST http://localhost:3000/users \
  -H "Content-Type: application/json" \
  -d '{"email":"test@test.com","name":"Test User"}'
```