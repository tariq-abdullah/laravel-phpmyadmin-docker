# Docker Compose file for Quick Setup of a Laravel Project with database management by phpmyadmin..

## Project Setup Guide

This guide will walk you through the steps to set up and run the project using Docker.

---

## Prerequisites

- Docker and Docker Compose installed on your machine.

---

## Steps to Run the Project

1. **Configure Environment Variables**
   - Edit or create the `.env` file in the root of your project.
   - Update the `PROJECT_NAME` variable to your desired project name.

2. **Start the Docker Containers**
   - Run the following command to start the services:
     ```bash
     docker-compose up
     ```

3. **Access the Application**
   - **Laravel Application**: Open your browser and go to [http://localhost:80](http://localhost:80).
   - **phpMyAdmin**: Access the database management tool at [http://localhost:81](http://localhost:81).
     - **Username**: `bn_myapp`
     - **Password**: (none)

4. **Access the Database Directly**
   - You can connect to the database directly at `localhost:3306`.

---

## Notes

- Ensure that the required directories (e.g., `./app`, `./database/mysql`) exist before running `docker-compose up`.
- If you encounter any issues, check the Docker logs for more details.

---

## Troubleshooting

- **Port Conflicts**: If ports `80`, `81`, or `3306` are already in use, update the `ports` configuration in `docker-compose.yml` to use different ports.
- **Missing `.env` File**: If the `.env` file is missing, create one by copying the `.env.example` file and updating the values.

---

## Support

For additional help, please refer to the official documentation or reach out to the project maintainers.
