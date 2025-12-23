# Network & Cyber Security - Fall 2025

## Content

- Lab 1: Security Compliance
- Lab 2: Threat Modeling
- Lab 3: Web Security
- Lab 4: Endpoint Security
- Lab 5: DevSecOps

## Instructions

1. Ensure you have docker and docker compose plugin installed

    ```bash
    docker -v
    docker compose version
    ```

1. Clone this repository

    ```bash
    git clone https://github.com/FIS-NCS/NCS-F25
    ```

1. Change into the project directory

    ```bash
    cd NCS-F25
    ```

1. [Before running any lab] Ensure you have the latest changes.

    ```bash
    git pull
    docker compose pull
    ```

1. Update `docker-compose.yaml` to serve files for lab `X` (i.e., `lab1`, `lab2`, etc.)

    ```yaml
    services:
      labenv:
          volumes:
            - ./labX:/app/workshop
    ```

1. Run the environment

    ```bash
    docker compose up -d
    ```

1. Access the lab at <http://localhost:3000>
