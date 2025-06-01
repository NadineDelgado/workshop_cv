# FastAPI Workshop - GitHub CI/CD Demo

This project demonstrates how to set up a CI/CD pipeline with GitHub Actions for a FastAPI application.

## Features

- FastAPI application with 3 endpoints
- Poetry for dependency management
- Pytest for testing
- GitHub Actions for CI/CD pipeline with test, build, and deploy stages

## Tecnologies

- Backend: FastAPI, Python
- Poetry
- Tests: Pytest
- CI/CD: GitHub Actions

## Pre requisites

Python
Poetry
Git

## Setup

1. Install Poetry if you don't have it already:
   ```
   curl -sSL https://install.python-poetry.org | python3 -
   ```

2. Install dependencies:
   ```
   poetry install
   ```

3. Run the application locally:
   ```
   poetry run uvicorn app.main:app --reload
   ```

4. Access the API documentation at http://localhost:8000/docs

## Tests

Run tests with:
```
poetry run pytest
```

## CI/CD Pipeline

The GitHub Actions workflow includes:

1. **Test**: Runs the test suite
2. **Build**: Builds a Docker image
3. **Deploy**: Deploys the application

This project implements a CI/CD pipeline with GitHub Actions that includes:

- **Testing**: Running unit tests with pytest
- **Linting**: Code quality check
- **Build**: Docker image creation
- **Deploy**: Test of the built image

The pipeline runs automatically with each push or pull request to the main branch.

All stages are executed on the GitHub runner machine. 

