# GLPI Docker Setup

## Requirements
- Docker Desktop installed
- Docker Compose installed
- At least 4GB of RAM available

## Installation Steps

1. **Clone or download the project** to your local machine
2. **Navigate to the project folder**:
   ```bash
   cd c:\Users\*********\Desktop\GLPI


3. Start the containers :

docker-compose up -d


4. Wait for the containers to initialize (this may take a few minutes)
## Accessing GLPI
- Open your browser and go to: http://localhost:8080
- Follow the GLPI installation wizard
## Database Configuration
The MySQL database is automatically configured with these credentials:

- Host : db
- Database name : glpidb
- Username : glpiuser
- Password : glpipassword
## Important Notes
- To stop the containers:

docker-compose down


To reset the installation (including database):
docker-compose down -v

## Trae AI
Used 1 context

docker-compose.yml 14-14

Here's a README.md file with instructions for running Docker and configuring the SQL server:

```markdown
# GLPI Docker Setup

## Requirements
- Docker Desktop installed
- Docker Compose installed
- At least 4GB of RAM available

## Installation Steps

1. **Clone or download the project** to your local machine
2. **Navigate to the project folder**:
   ```bash
   cd c:\Users\elmessonjesus\Desktop\GLPI
 ```
```

3. Start the containers :
   
   ```bash
   docker-compose up -d
    ```
4. Wait for the containers to initialize (this may take a few minutes)
## Accessing GLPI
- Open your browser and go to: http://localhost:8080
- Follow the GLPI installation wizard
## Database Configuration
The MySQL database is automatically configured with these credentials:

- Host : db
- Database name : glpidb
- Username : glpiuser
- Password : glpipassword
## Important Notes
- To stop the containers:
  
  ```bash
  docker-compose down
   ```
- To reset the installation (including database):
  
  ```bash
  docker-compose down -v
   ```
## Changing Default Passwords
For security, change these default passwords in the docker-compose.yml file:

1. GLPI_DB_PASSWORD
2. MYSQL_ROOT_PASSWORD
3. MYSQL_PASSWORD
## Backup Recommendations
Regularly backup these folders:

- ./glpi/files - Contains uploaded files
- ./glpi/mysql - Contains database files
- ./glpi/config - Contains configuration files