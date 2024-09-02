# Pando Services - NestJS Backend

This project is a NestJS backend for managing EV charging stations.

## Prerequisites

- [Docker](https://www.docker.com/get-started) (version 20 or later)
- [Docker Compose](https://docs.docker.com/compose/install/) (version 1.29 or later)

## Local Development

1. **Clone the Repository:**

   ```bash
   git clone git@gitlab.com:pando_electric/pando-services.git
   cd pando-services
   ```

2. **Create and Configure the `.env.x` File:**

   **- For Development**:

   Copy the `.env.development.example` file to `.env.development`:

   ```bash
   cp .env.development.example .env.development
   ```

   Edit the `.env.development` file to set your local environment variables.

   **- For Production**:

   Copy the `.env.production.example` file to `.env.production`:

   ```bash
   cp .env.production.example .env.production
   ```

   Edit the `.env.production` file to set your prod environment variables.

3. **Build and Start the Application:**

   ```bash
   docker-compose up --build
   ```

   This will build the Docker image and start the containers.

4. **Access the Application:**

   Open your browser and go to `http://localhost:3000/api` to view the application and `http://localhost:3000/api-doc` to access API documentation.

5. **Stopping the Application:**

   ```bash
   docker-compose down
   ```

6. **Run unit tests:**

   ```bash
   docker-compose run --rm app npm run test
   ```
