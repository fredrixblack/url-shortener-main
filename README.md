# URL Shortener System

This repository serves as the main project for a microservice-based URL shortening system. It includes all necessary services as Git submodules.

## System Architecture

The URL Shortener system consists of the following microservices:

- **API Gateway**: Front-facing service that routes requests to appropriate services
- **Auth Service**: Handles user authentication and authorization
- **URL Shortening Service**: Core service that manages URL shortening and redirection

## Repository Structure

```
url-shortener-main/
  ├── api-gateway/            # API Gateway service submodule
  ├── auth-service/           # Authentication service submodule
  ├── url-shortening-service/ # URL Shortening service submodule
  ├── .gitmodules             # Submodule configuration
  └── README.md               # This file
```

## Getting Started

### Prerequisites

- Git
- Docker and Docker Compose (for running the services)

### Clone the Repository

To clone this repository with all submodules:

```bash
git clone --recurse-submodules https://github.com/fredrixblack/url-shortener-main.git
cd url-shortener-main
```

If you've already cloned the repository without the submodules:

```bash
git submodule init
git submodule update
```

### Updating Submodules

To update all submodules to their latest versions:

```bash
git submodule update --remote
```

## Development Guidelines

1. Each service should be developed in its own repository
2. The main repository should only be used to track submodule versions
3. For changes to individual services, navigate to the service directory and follow standard Git workflow
4. After committing changes to a service, update the submodule reference in the main repository

## Deployment

Instructions for deploying the entire system can be found in the deployment documentation.

## License

none

## Contact

fredrix black
