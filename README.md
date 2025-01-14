# setup_databases
Setup databases on Ubuntu server with MySQL, PostgreSQL, MongoDB, Redis, and Elasticsearch.

## Prerequisites
- Ubuntu server
- Root access
- Internet connection

## PostgreSQL 
1. Update package list:
    ```bash
    sudo apt-get update && sudo apt-get upgrade -y 
    ```
2. Install PostgreSQL and additional features:
    ```bash
    sudo apt-get install postgresql postgresql-contrib
    ```
3. Login to PostgreSQL:
    ```bash
    sudo -u postgres psql
    ```
4. Create a user:
    ```sql
    CREATE USER username WITH PASSWORD 'password';
    ```
5. Create a database:
    ```sql
    CREATE DATABASE dbname;
    ```
6. Grant privileges to the user on the database:
    ```sql
    GRANT ALL PRIVILEGES ON DATABASE dbname TO username;
    ```
7. Exit PostgreSQL:
    ```sql
    \q
    ```