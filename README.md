# Vecap Data Warehouse

This project is an enterprise data warehouse design that leverages Directed Acyclic Graphs (DAGs) for efficient data processing and management.

## Table of Contents
- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Vecap Data Warehouse project aims to provide a robust and scalable data warehouse solution for enterprise-level data management. It utilizes Directed Acyclic Graphs (DAGs) to ensure efficient data flow and processing.

## Technologies Used
- **Python**: The primary programming language used for data processing and management.
- **Airflow**: For orchestrating data workflows using DAGs.
- **PostgreSQL**: As the primary database for storing data warehouse information.
- **Docker**: For containerizing applications and ensuring consistent environments.

## Architecture
The architecture of the Vecap Data Warehouse is designed to handle large volumes of data efficiently. It includes:
- **Data Ingestion Layer**: Responsible for collecting data from various sources.
- **Data Processing Layer**: Utilizes Airflow DAGs to process and transform data.
- **Data Storage Layer**: Stores processed data in a PostgreSQL database.
- **Data Access Layer**: Provides APIs and tools for accessing and analyzing data.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- **Python 3.x** installed on your machine.
- **Docker** installed for containerization.
- **PostgreSQL** database setup.

## Usage
To set up and run the project, follow these steps:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/Shamoo100/vecap_datawarehouse.git
   cd vecap_datawarehouse
   ```

2. **Set up the environment**:
   ```sh
   python -m venv env
   source env/bin/activate   # On Windows use `env\Scripts\activate`
   ```

3. **Install dependencies**:
   ```sh
   pip install -r requirements.txt
   ```

4. **Start Docker containers**:
   ```sh
   docker-compose up
   ```

5. **Run Airflow**:
   ```sh
   airflow initdb
   airflow webserver -p 8080
   airflow scheduler
   ```

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License.
