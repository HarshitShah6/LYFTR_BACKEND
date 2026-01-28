# LYFTR Backend

## Applicant Information

**Name:** Harshit Shah  
**Roll No:** 10322210049  
**Position Applied:** Full Stack Developer at Lyftr

---

## Overview

This is a backend application built with FastAPI for the Lyftr platform. The project includes API endpoints, database models, metrics, and comprehensive testing.

## Project Structure

```
lyftr-backend/
├── app/
│   ├── __init__.py
│   ├── main.py           # FastAPI application entry point
│   ├── config.py         # Configuration settings
│   ├── models.py         # Database models
│   ├── storage.py        # Storage operations
│   ├── metrics.py        # Metrics tracking
│   └── logging_utils.py  # Logging utilities
├── tests/
│   ├── conftest.py
│   ├── test_messages.py
│   ├── test_stats.py
│   └── test_webhook.py
├── requirements.txt      # Python dependencies
├── docker-compose.yml    # Docker Compose configuration
├── dockerfile            # Docker image configuration
├── makefile              # Make commands
└── pytest.ini            # Pytest configuration
```

## Setup Instructions

### Prerequisites
- Python 3.11+
- Virtual environment (myenv)
- Docker (optional)

### Installation

1. Activate the virtual environment:
```bash
source myenv/bin/activate  # On Windows: myenv\Scripts\Activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Running the Application

Start the server:
```bash
uvicorn app.main:app --reload
```

The API will be available at `http://localhost:8000`

### Running Tests

Execute the test suite:
```bash
pytest
```

### Docker

Build and run with Docker Compose:
```bash
docker-compose up --build
```

## Features

- RESTful API endpoints
- Database integration with SQLAlchemy
- Prometheus metrics integration
- Comprehensive logging
- Full test coverage with pytest
- Docker containerization support

## Technologies Used

- **Framework:** FastAPI
- **Database:** SQLAlchemy with async support (aiosqlite)
- **Testing:** Pytest
- **Monitoring:** Prometheus Client
- **HTTP Client:** HTTPX
- **Server:** Uvicorn

## Contact

For inquiries or feedback, please reach out regarding this application.

---

**Last Updated:** January 28, 2026
