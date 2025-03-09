# Rodiun iPaaS

Integration Platform as a Service solution for connecting legacy systems with modern applications.

## Overview

Rodiun iPaaS is a comprehensive integration platform designed to serve as a middleman between legacy systems and modern applications. It provides a robust data integration and transformation platform that enables seamless connectivity across diverse systems.

## Key Features

- Agent-based architecture for data extraction, transformation, and loading
- Workflow orchestration via Apache Airflow with Kafka-based messaging
- Integration routing via Apache Camel for HTTP API calls and SFTP transfers
- Multi-tenant database design with schema-per-account isolation
- Modern React frontend with interactive workflow visualization
- Comprehensive role-based access control system

## Project Structure

```
├── airflow/            # Airflow components for workflow orchestration
├── backend/            # FastAPI backend application
├── frontend/           # React frontend application
├── docker-compose.yml  # Docker Compose configuration
└── documents/          # Project documentation
```

## Getting Started

### Prerequisites

- Docker and Docker Compose
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jarod-AI/Rodiun_iPaaS.git
   cd Rodiun_iPaaS
   ```

2. Start the services using Docker Compose:
   ```bash
   docker-compose up -d
   ```

3. Access the services:
   - Backend API: http://localhost:8000/api/v1/docs
   - Frontend: http://localhost:3000
   - Airflow: http://localhost:8080

## Development

### Backend Development

The backend is built with FastAPI and uses SQLAlchemy for database operations. To set up the development environment:

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

### Frontend Development

The frontend is built with React, TypeScript, and Tailwind CSS. To set up the development environment:

```bash
cd frontend
npm install
npm run dev
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.