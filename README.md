# Docker Compose PHP Development Environment

This repository contains a simple Docker Compose setup for PHP development. It includes PHP 8.1, Composer for managing dependencies, and MySQL 5.7 for database operations.

## Prerequisites

Make sure you have Docker and Docker Compose installed on your system.

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Usage

1. Clone this repository:

    ```bash
    git clone https://github.com/ulreck-drulk/composer_platzi.git
    ```

2. Navigate into the cloned repository:

    ```bash
    cd composer_platzi
    ```

3. Start the Docker containers:

    ```bash
    docker compose up -d
    ```

4. Access your PHP application at [http://localhost:9000](http://localhost:9000).

## Services

- **app**: PHP 8.1 server running with PHP-FPM, serving files from the `/var/www/html` directory.
- **composer**: Composer container for managing PHP dependencies. It installs dependencies defined in `composer.json`.
- **db**: MySQL 5.7 database container with a pre-defined database `projectdb`.

## Configuration

You can configure the PHP application environment variables in the `docker-compose.yml` file under the `app` service.

## Development

You can edit your PHP code locally, and changes will be reflected immediately as the application is served from the host directory.

## Disclaimer

This Docker Compose environment has not been tested extensively and is intended solely as a practice exercise to improve Docker skills. Use it at your own risk.

## License

This project is licensed under the [MIT License](LICENSE).
